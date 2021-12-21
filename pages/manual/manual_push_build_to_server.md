---
title: Pushing builds to server
tags: [publishing]
keywords: AWS, Amazon, command line, pushing build
last_updated: July 3, 2016
summary: "You can push your build to AWS using commands from the command line. By including your copy commands in commands, you can package all of the build and deploy process into executable scripts."
sidebar: manual_sidebar
permalink: manual_push_build_to_server.html
folder: manual
---


## Pushing to AWS S3

If you have the AWS Command Line Interface installed and are pushing your builds to AWS, the following commands show how you can build and push to an AWS location from the command line:

```
aws s3 cp ~/users/tjohnson/projects/manualproject/ s3://[aws path]docpath/manualproject --recursive

aws s3 cp ~/users/tjohnson/projects/anotherdocproject2/ s3://[aws path]docpath/anotherdocproject --recursive
```

The first path in the argument is the local location; the second path is the destination.

## Pushing to a regular server

If you're pushing to a regular server that you can ssh into, you can use `scp` commands to push your build. Here's an example:

```
scp -r /users/tjohnson/projects/manualproject/ name@domain:/var/www/html/manualproject
```

Similar to the above, the first path is the local location; the second path is the destination.

{% include links.html %}
