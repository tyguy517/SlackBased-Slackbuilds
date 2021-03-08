tested on slackware 14.2 and works, just one warning:

> WARNING:  /usr/share/man (with possibly not gzipped man pages) detected

on slackware current (probably)

```bash
rm -f
/build/tmp/SBo/package-ZeroTierOne/usr/share/man/man8/zerotier-one.8.gz
cat doc/zerotier-one.8 | gzip -9
> /build/tmp/SBo/package-ZeroTierOne/usr/share/man/man8/zerotier-one.8.gz
mkdir -p /build/tmp/SBo/package-ZeroTierOne/usr/share/man/man1
rm -f
/build/tmp/SBo/package-ZeroTierOne/usr/share/man/man1/zerotier-idtool.1.gz
rm -f
/build/tmp/SBo/package-ZeroTierOne/usr/share/man/man1/zerotier-cli.1.gz
cat doc/zerotier-cli.1 | gzip -9
> /build/tmp/SBo/package-ZeroTierOne/usr/share/man/man1/zerotier-cli.1.gz
cat doc/zerotier-idtool.1 | gzip -9
> /build/tmp/SBo/package-ZeroTierOne/usr/share/man/man1/zerotier-idtool.1.gz
mkdir: cannot create directory
‘/build/tmp/SBo/package-ZeroTierOne/usr/doc/ZeroTierOne-1.4.6’: No such
file or directory
mkdir: cannot create directory ‘/’: File exists
```
