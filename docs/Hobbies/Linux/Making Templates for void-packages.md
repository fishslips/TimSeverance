### Void Packages Manual
https://github.com/void-linux/void-packages/blob/master/Manual.md#namingconventions

### Instructional Video
https://www.youtube.com/watch?v=p_gcoKEjGho

### Checksums
11:09:49 PM - fishslips: Hey everyone, I'm learning how to do templates for void-packages, and I'm a little confused about the checksum part. For the checksum, am I supposed to use an official checksum provided by the developers or am I supposed to generate the checksum for the distfiles and then use that?
11:10:11 PM - xmsz [~xmszkn@user/xmszkn] entered the room.
11:11:39 PM - solarsparq has left the room (Quit: Ping timeout: 276 seconds).
11:12:48 PM - abby: if the devs provide a sha256sum, it could be used
11:12:57 PM - abby: usually it's easier to generate locally
11:13:56 PM - fishslips: what if they only provide it for compiled binaries? I'm obviously generating a template for the source to be compiled, so I was pretty sure those would be different, but I wasn't sure exactly what the checksum field is supposed to be in the template file.
11:14:08 PM - abby: then generate it locally
11:14:26 PM - fishslips: Okay slick, that's easy enough
11:14:28 PM - abby: xgensum -i pkgname is easiest
11:14:49 PM - fishslips: thank you for the help!
11:16:46 PM - solarsparq [~quassel@108.174.50.37] entered the room.
11:16:49 PM - fishslips: oh sorry, last question
11:16:56 PM - fishslips: I just do it on the tar.gz right?
11:18:00 PM - abby: usually
11:18:40 PM - abby: in rare cases those tarballs are generated on-the-fly, so they have a different checksum every time. in that case, a content checksum is needed
11:19:28 PM - fishslips: How would I handle that?
11:20:23 PM - abby: xgensum -ci and let it do its thing
11:20:41 PM - fishslips: awesome
11:20:45 PM - fishslips: thanks a ton for the help!