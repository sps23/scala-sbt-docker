Forked from [hseeberger/scala-sbt](https://github.com/hseeberger/scala-sbt)

# Scala and sbt Dockerfile

This repository contains **Dockerfile** of [Scala](http://www.scala-lang.org) and [sbt](http://www.scala-sbt.org).


## Base Docker Image ##

* [openjdk:8](https://hub.docker.com/_/openjdk)


## Usage in Pipelines ##

```
image: bitbucketpipelines/scala-sbt:scala-2.12

pipelines:
  default:
    - step:
        script:
          - sbt test
```

## Extending or using different Scala or SBT versions
Feel free to fork this repo and change the `SCALA_VERSION` in `SBT_VERSION` values in the Dockerfile.

## Contribution policy ##

Contributions via Bitbucket pull requests are gladly accepted from their original author. Along with any pull requests, please state that the contribution is your original work and that you license the work to the project under the project's open source license. Whether or not you state this explicitly, by submitting any copyrighted material via pull request, email, or other means you agree to license the material under the project's open source license and warrant that you have the legal authority to do so.


## License ##

This code is open source software licensed under the [Apache 2.0 License]("http://www.apache.org/licenses/LICENSE-2.0.html").