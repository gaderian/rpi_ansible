RPi Change User
=========

Will create a new user with a random password and a copy of the current users public key in its known hosts file. The root user will also have a new password set.

Role Variables
--------------
| Name                | Default Value | Description                                                   |
|---------------------|---------------|---------------------------------------------------------------|
| `username`          |               | The name of the new user                                      |
| `rpi_disable_pi`    | true          | Will lock the pi user if true                                 |
| `rpi_password_path` | /tmp/         | The path where files containing the new passwords are written |

NOTE: `rpi_password_path` should be pointing to an encrypted location e.g. a mounted [veracrypt] volume.

[veracrypt]: https://www.veracrypt.fr
