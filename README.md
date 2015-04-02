discourse-bbcode-color
======================

A Discourse Plugin to support Font Awesome text inline.

Usage
=====

In your posts, surround text with `[fa-iconname]`. C

Installation
============

* Add the plugin's repo url to your container's yml config file

```yml
hooks:
  after_code:
    - exec:
        cd: $home/plugins
        cmd:
          - mkdir -p plugins
          - git clone https://github.com/discourse/docker_manager.git
          - git clone https://github.com/sgcoldsun/discourse-inline-icons.git
```

* Rebuild the container

```
cd /var/docker
git pull
./launcher rebuild app
```

License
=======

MIT

