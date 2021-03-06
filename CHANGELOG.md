# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2018-11-24
### Added
- config:dump -- Dump config settings (mostly for quick reference)
- config:menu -- Set config easier than before
- self:migrate -- Migrate from pre-v1
- server:backup -- Now schedulable
### Changed
- All Commands -- Complete rewrite, now using a database
- server:fix -- Better scheduling

## [0.0.18] - 2018-11-19
### Fixed
- fivem:install
- fivem:update -- The collective changed some stuff.

## [0.0.17] - 2018-02-01
### Added
- server:restart -- Restart the server with one command, instead of two
### Fixed
- server:create -- Small bug that wouldn't allow path to be manually set if the server:path was set
- Some typos

## [0.0.16] - 2018-01-31
### Added
- fivem:license -- save license for starting server
### Changed
- server:start -- now will automatically include license key, if set
### Fixed
- server:path -- Wouldn't let you set a new path
- server:create -- Didn't check if server existed, properly
- Some typos

## [0.0.15] - 2017-12-19
### Added
- server:rename -- renames a server
- BaseCommand -- cleaner code
- Prompts for server name will now have auto-complete
### Changed
- Refactored all commands -- to use BaseCommand
### Fixed
- Some typos
### Removed
- illuminate/filesystem from composer.json [#6](https://github.com/TNovalis/FiveM-ServerManager/pull/6)

## [0.0.14] - 2017-11-23
### Changed
- Updated laravel-zero/framework for friendlier error messages
### Removed
- composer.lock

## [0.0.13] - 2017-11-22
### Added
- server:fix -- fixes crashed servers - **scheduled**

## [0.0.12] - 2017-11-17
### Fixed
- A totally not obvious copy-paste job

## [0.0.11] - 2017-11-17
### Added
- server:backup -- backs up a server
- server:delete -- deletes server after running a server backup unless you use `--no-backup`
### Fixed
- fivem:update -- some dev testing code was left in

## [0.0.10] - 2017-11-17
### Changed
- almost all commands, cleaning up
### Fixed
- server:say -- slight issue

## [0.0.9] - 2017-11-16
### Added
- server:console -- see the server console
- server:say -- send a message to the console
### Changed README
- Added support
### Fixed
- server:list -- now checks status of server process
- server:create -- shut git the fu*k up
- server:path -- now tells you the path if it is set and a paht isn't provided
- server:stop -- now sends message to server, disablable

## [0.0.8] - 2017-11-15
### Fixed
- Stop Command signature throwing error

## [0.0.7] - 2017-11-15
### Changed
- Storage location for easier updating

## [0.0.4] - 2017-11-15
### Added
- Laravel-Zero
- The initial commands
