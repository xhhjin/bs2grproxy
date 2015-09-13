BS2GRProxy Introduction

# Introduction

A small app runs on Google App Engine as a reverse proxy to a specific site.

# Features

1. Reverse proxy
2. Web pages, css/js and media files can be redirected to different hosts
3. Configurable through Google App Database view 

# How to use

1. Download the source package
2. Modify app name in app.yaml
3. Upload the app
4. Enjoy 

# Configuration

You can set default config in bs2grpconfig.py. But how ever it's not encouraged to modify the source code unless you understand it.

After the first run on app engine, a data entry will be created in table "BS2GRPConfig". You can set run time options there using Data View in app admin page.

# Options in BS2GRPConfig

target_host: HTML target url.
static_host: Static target url.
cssjs_redirect: Redirect css/js files to static host. Including: .css .js
media_redirect: Redirect media files to static host. Including: .jpg .jpeg .gif .png .avi .mov .mp3 .rm .rmvb .qt

