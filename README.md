# nextcloud-xl

This is the [`nextcloud:apache`](https://hub.docker.com/_/nextcloud) image, with a bunch of extra additions. This image is NOT SMALL - it weighs in at about 1.8 gigabytes. It is based on the [`full`](https://github.com/nextcloud/docker/tree/master/.examples/dockerfiles/full/apache) example Dockerfile from Nextcloud, but with even more things added:

- [aria2](https://aria2.github.io/) and [youtube-dl](https://youtube-dl.org/) (in case you want to run [ocDownloader](https://github.com/e-alfred/ocdownloader) or [ncdownloader](https://github.com/shiningw/ncdownloader))
- clamdscan from [ClamAV](https://www.clamav.net/) (in case you want to run [files_antivirus](https://github.com/nextcloud/files_antivirus)) (additional ClamAV container requred, I recommend [tiredofit/clamav](https://hub.docker.com/r/tiredofit/clamav))
- [FFmpeg](https://www.ffmpeg.org/) (for video thumbnails)
- [Ghostscript](https://www.ghostscript.com/) (for document previews)
- [ImageMagick](https://imagemagick.org/) (for image previews)
- [LibreOffice](https://www.libreoffice.org/) (for even more document previews)
- [p7zip](http://p7zip.sourceforge.net/) and [unrar](https://linux.die.net/man/1/unrar) (for opening archives)
- smbclient from [Samba](https://www.samba.org/) (for connecting to Windows shares)
- [Supervisor](http://supervisord.org/) (so you don't have to run a separate cron container)

## Links

- [nextcloud-xl on Docker Hub](https://hub.docker.com/r/jordemort/nextcloud-xl)
- [nextcloud-xl on GitHub](https://github.com/jordemort/nextcloud-xl)
