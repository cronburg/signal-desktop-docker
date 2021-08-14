FROM archlinux

RUN pacman --noconfirm -Syyuu
RUN pacman --noconfirm -S signal-desktop
RUN pacman --noconfirm -S strace

ARG uid
ARG gid

RUN groupadd --gid $gid signal
RUN useradd -m --gid $gid --uid $uid signal

VOLUME ["/home/signal/.config"]

RUN chown -R $uid:$gid /home/signal/.config

