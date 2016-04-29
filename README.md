# alpine-routersploit
alpine-routersploit

This Docker image allow to run the latest routersploit on Alpine Linux.

Pull the image with:
docker pull fcolista/alpine-routersploit

Run docker image with:
docker run -it fcolista/alpine-routersploit

Note:
If you are running with a grsec kernel, you should disable those features:
chroot_deny_chmod
chroot_deny_mknod

With alpine host, you can do it by decommenting from /etc/conf.d/docker:

#disable_grsec="chroot_deny_chmod chroot_deny_mknod"
and then restart docker:
rc-service docker restart

Enjoy,
Francesco
