# Dropbox via systemd

Also known as, _systemd-dropbox_; provides a means to run someones Dropbox daemon as a system
service.

## Rational

If you are running a server where you wish to allow a user's Dropbox files to be synced before the
user is logged in.

## Usage

To enable boot-time launching of Dropbox via systemd, call `systemctl enable dropbox@$username` as
root, or via `sudo`, where `$username` is the user's login name.  To immediately start the service,
call `systemctl start dropbox@$username` as root, or via `sudo`.
