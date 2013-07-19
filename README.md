# Rubeque [![Build Status](https://api.travis-ci.org/SciMed/rubeque.png?branch=develop)](https://api.travis-ci.org/SciMed/rubeque.png?branch=develop)

Rubeque is an interactive problem website for learning Ruby.

## Contributing

Anyone interested in contributing should check out
the [Issues](https://github.com/SciMed/rubeque/issues) page for ideas
on what to work on.

## Setup instructions for running locally

* Download and install [rvm](http://beginrescueend.com/).
* Download and install [mongodb](http://www.mongodb.org/).
* Enter the rubeque directory from the command line and follow the rvm instructions to install ruby 1.9.3
* To install debugger:

  ```
      gem install debugger-linecache -v '1.1.2' -- --with-ruby-include=$rvm_path/src/ruby-1.9.3-p429/
      gem install ruby-debug19
  ```

* Start up your mongodb, if you don't have autostart:

        mongod
* Run "bundle install" to install the necessary gems
* Run `rake secret` and put the generated token in an environment variable
  named SECRET\_TOKEN in your .bashrc (don't forget to source it!)
* For the first time use, you will need to load the problem data. Run "rake db:seed"
* Run `rails server`

## Contributors

* [David Davis](https://github.com/daviddavis) (daviddavis)
* [Kamal Bennoune](https://github.com/kbennoune) (kbennoune)
* [Joe Peck](https://github.com/fatcatt316) (fatcatt316)
* [Michael Stalker](https://github.com/mstalker) (mstalker)
* [Joseph Jaber](https://github.com/josephjaber) (josephjaber)
* [Edward Anderson](https://github.com/nilbus) (nilbus)
* [Anatoli Makarevich](https://github.com/makaroni4) (makaroni4)
* [Rogelio Guzman](https://github.com/rogeliog) (rogeliog)
* [Michaux Kelley](https://github.com/mkelley33) (mkelley33)

## Acknowledgements

* [SciMed Solutions, Inc](http://www.scimedsolutions.com) for providing the time and resources necessary to make this.
* [4clojure](http://www.4clojure.com) for providing advice and support.
* [envylabs](https://github.com/envylabs) for their Ruby Conf presentation on sandboxing
* [Nick Markwell](https://github.com/duckinator) for his help in sandboxing

## License

The source code for rubeque is available under the [MIT License](http://www.opensource.org/licenses/MIT).
