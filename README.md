# mmpv

MPD-aware mpv. A simple mpv wrapper for avoiding overlapping of music.


## Idea

`mmpv` behaves identically to `mpv`, but before starting, it pauses MPD and kills all other instances of itself.

Additionally, it provides "quiet" option (`mmpv -q …`) which runs `mpv` on background, in a detached `tmux` session, which you can attach to later with `mmpv -a`.


## Configuration

Following environment variables are read:

    MMPV_PIDFILE (default is /tmp/mmpvpid)
    MMPV_SESSION (default is MMPV)
    MMPV_PLAYER  (default is mpv)


## Dependencies

  * `tmux`
  * MPD & `mpc`
  * `mpv`
