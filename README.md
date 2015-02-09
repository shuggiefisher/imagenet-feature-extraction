



# The Pipeline

![Pipeline diagram](http://goo.gl/jdE5wV)


## Imagenet feature extraction

This repo contains a [brain4k](https://github.com/shuggiefisher/brain4k) pipeline for extracting image features using a network trained on the imagenet database.

to execute the pipeline within a docker container:

```
sudo docker run -ti tleyden5iwx/caffe-cpu-master /bin/bash
pip install git+https://github.com/shuggiefisher/brain4k.git
git clone https://github.com/shuggiefisher/imagenet-feature-extraction.git local-path-to-this-repo
brain4k local-path-to-this-repo
```

### Requirements
- [brain4k](https://github.com/shuggiefisher/brain4k)
- caffe, including python wrappers

Installing caffe is quite involved, so you may find it easier to use a
[caffe docker image](https://registry.hub.docker.com/u/tleyden5iwx/caffe/)
