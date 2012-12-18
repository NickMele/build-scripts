# Ant Build Script
This build script is used to create releases of source code for a project.

## Process
1. Asks for version number of release
2. Creates release directory if does not exist
3. Moves previous release into new directory with version number (./release/###)
4. Copies files from source folder to release/latest folder
5. Minifies stylesheets using yui-compressor
6. Minifies scripts using closure compiler
7. Optimizes images (png and jpg separately)
8. Stores version information for current release
9. [OPTIONAL] Tags git repo with version number

## Future implementations
- Log each release to track history of builds
- Implement option to tag in git or svn
- Update boilerplate with references to any new files / name changes
