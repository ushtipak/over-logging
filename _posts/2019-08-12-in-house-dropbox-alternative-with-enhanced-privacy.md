---
title: "In-house Dropbox alternative with enhanced privacy"
categories: [golang, aes]
---

You've watched Black Mirror and Mr Robot and categorize them as Sci-Fi?

Go back to Facebook, write some generic quote, like a few funny videos and have
a nice day...


# Information

Our data is never safe and the only thing we can do is to make it harder for
someone to obtain it

Mr Josh Shaul, CTO with Application Security, nicely framed it:

> "Only hardcore security professionals think about the fact that you can never
be totally secure. The only thing you can do is build the fence higher and
higher so that eventually it’s not worth it to climb over."

Picking "123456Seven" as your password, in comparison to
"0mG  l3mmmy tRY the POOLing 0pt !?!", makes the difference in whether the
attacker will crack it in a few minutes, or in a hundred lifetimes

Sadly, we're far from vigilant, and we even share our data with numerous
services for pure convenience

Having your files available on multiple devices is of course beneficial, that's
why people opt to use services like pCloud, Sync, Dropbox,  {Google ,One}Drive
– broadening the question with – who can access your data, beside you?


## Just a glimpse

Let's dissect the most popular of the beforementioned, Dropbox

End-to-end encryption is not implemented and their official
[Privacy Policy](https://www.dropbox.com/privacy) honestly states:
`We may share information` ...

Further more – your files aren't truly private –
`Dropbox personnel will, on rare occasions, need to access users’ file content`
([more detail](https://help.dropbox.com/accounts-billing/security/file-access))

You've got nothing to hide, good, but that doesn't mean that someone should be
able to look into your files without your consent, no matter how insignificant
your shared "list of things to pack" might be


# Mention this to me

[Disposition](https://github.com/ushtipak/disposition), named after a Tool
song, solves some of the cited problems

It lacks automated sync that Dropbox has (might be added in the future), fancy
web interface (has none, actually) and link sharing capabilities, but
compensates by giving you full control of your data, completely secured with
AES 256-bit encryption

Running Disposition on a free GitHub private repo, compared to Dbox:

|                                | Dropbox | Disposition |
|--------------------------------|---------|-------------|
| Possible unwanted decryption   | ✔       | ✗           |
| Info shared with third-parties | ✔       | ✗           |
| Transparent file processing    | ✗       | ✔           |
| End-to-end encryption          | ✗       | ✔           |
| Open source                    | ✗       | ✔           |
| Free storage (GB)              | 2       | 100         |


## And watch the weather change

Unlike other similar software – Disposition keeps encrypted files locally and
syncs them to a remote repo

Entire process is trivial: each file in target directory (and it's sub-dirs) is
compared to the state of previously enrolled entries and handled accordingly

If it's a new one – it's MD5 will be calculated and it's encrypted counterpart
will be created in pre-configured root, with an obfuscated name; and both will
be added to a sqlite DB for the future reference

If, however, the file is purely updated, it'll be re-encrypted with formerly
delegated obfuscated name and it's checksum will be populated to the state DB

{% highlight plaintext %}
m@phoenix-person:/opt/disposition$ tree
.
├── disposition-state.db
├── disposition.yml
├── plain
│   ├── 2do
│   ├── acc
│   │   ├── valhalla---ions-flmr
│   │   ├── valhalla---parabola-flmr
│   │   ├── valhalla---parabola-jntr
│   │   ├── valhalla---parabola-strs
│   │   ├── valhalla---parabola-td
│   │   └── valhalla---suggestive-flmr
│   └── transfer
└── remote
    ├── 1afda9f9-21c9-4ca9-aa5d-602e9bfaa01e
    ├── 1e214c13-db6c-494f-a5ed-a0533a17947a
    ├── 5f769b96-5fc1-43c9-a61f-6941dac30397
    ├── 83280991-66a6-4267-8e62-e4f211166c2f
    ├── 8951290d-5126-4556-ad00-a0d638e7fe4b
    ├── a253e032-a7a9-4575-ad72-c97f8d2b8cc8
    ├── cb693879-5319-4221-919d-fac96401abfa
    ├── d7e83ff8-5ed5-4a69-8795-eb37e6091c13
    └── f785d6c2-6919-41da-959f-10eff3664739

3 directories, 19 files
{% endhighlight %}

> plain and encrypted files, side-by-side


Entire file path is preserved, but the encrypted blob is stored as a UUID in a
flat structure, not making it easier for a potential attacker (there is no way
to differentiate files by their name), and the state DB has all the mappings:

![Disposition state]({{ site.url }}{{ site.baseurl }}/assets/2019-08-12-in-house-dropbox-alternative-with-enhanced-privacy/state-db.png)


Pull process is basically the same motion in reverse and there is also an
option of a full data restore, if you're adding a new workstation to the mix


# POCs or It Didn't Happen

Disposition was developed with itself as the version-control system, so that
core concepts were tested in actual dev, prior to it's "release" (initial 62
commits)

![Is this a pigeon]({{ site.url }}{{ site.baseurl }}/assets/2019-08-12-in-house-dropbox-alternative-with-enhanced-privacy/dev-state.jpg)


However, there are no binaries atm, nor the bootstrap "wizard" for populating
configs and gluing remote repos, but it might be added in the future too

Configuration (defaults to `/opt/disposition/disposition.yml`) is stored in
YAML where the following needs to be provided:

{% highlight plaintext %}
---
root:
  plain: "/opt/disposition/plain"
  encrypted: "/opt/disposition/remote"
secret:
  key: "░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░"
  state: "/opt/disposition/disposition-state.db"
  obfuscated: "cb693879-5319-4221-919d-fac96401abfa"
{% endhighlight %}


Comprise a random key of 32 bytes, keep it safe and disposition your files

