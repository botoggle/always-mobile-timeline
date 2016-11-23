# Always Mobile Timeline for Discourse

Some of us don't like a fifth of the browser window being used up to show an adorable little secondary scroll-bar at all times. This plugin fixes that, by having Discourse always use the "mobile" timeline display. No settings, no support, no problem.

## Usage
Plug-and-play. 

## Installation
* Add this repo to your app.yml, as usual.
```yml
hooks:
  after_code:
    - exec:
        cd: $home/plugins
        cmd:
          - mkdir -p plugins
          - git clone https://github.com/discourse/docker_manager.git
          - git clone https://github.com/botoggle/always-mobile-timeline-discourse.git
```
* Rebuild the container.
```bash
cd /var/discourse
./launcher rebuild app
```
* Wow, you did it!

## License
Good ol' GNU GPL 2.