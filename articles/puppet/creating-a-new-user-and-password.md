# Making a new User and password in Puppet

Create the user manually, and look at the file `/etc/shadow`
You'll see something like this
```
root:$6$tUH1hyAU$AT8QppJ6JZEFPgLga62qlkxTZ2jDHDcyP5FCxcYPqCU8nAaXd0eJtD4df1fSCyxQGtALgx3JI.vjVZ6s2i8Eh1:15537:0:99999:7:::
```

The password is here `$6$tUH1hyAU$AT8QppJ6JZEFPgLga62qlkxTZ2jDHDcyP5FCxcYPqCU8nAaXd0eJtD4df1fSCyxQGtALgx3JI.vjVZ6s2i8Eh1`

```puppet
user { 'thomaswelton':
    comment => 'Thomas Welton',
    home    => '/home/thomaswelton',
    shell   => '/bin/zsh',
    managehome => 'true',
    password  => '$6$YiYH0Utf$qM7MSnx29gvLZE3l8xMYdgr4P6wirdCkgSmF7zLkzltgXnVrXK6xtjFAb6faGCNO9a4xywwTSPuyvKwzCc5P5.'
}
```
