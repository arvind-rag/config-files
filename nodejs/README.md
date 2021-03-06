# Node.js

## Global packages

- [create-react-app](https://github.com/facebook/create-react-app) - React boilerplate
- [fixpack](https://www.npmjs.com/package/fixpack) - Sort package.json
- [grunt](https://gruntjs.com/) - Task runner
- [gulp](https://gruntjs.com/) - Streaming build system
- [hexo](https://hexo.io/) - Static site generator
- [mozjpeg](https://github.com/imagemin/mozjpeg-bin) - JPEG optimizer
- [npm-check-updates](https://www.npmjs.com/package/npm-check-updates) - Upgrade package.json dependencies
- [ntl](https://www.npmjs.com/package/ntl) - List and run npm tasks
- [prettier](https://prettier.io/) - Code formatter
- [svgexport](https://github.com/shakiba/svgexport) - SVG → PNG/JPEG vonverter
- [svgo](https://github.com/svg/svgo) - SVG optimizer

```
npm install -g create-react-app fixpack grunt-cli gulp hexo-cli mozjpeg npm-check-updates ntl prettier svgexport svgo
```

## npm

```bash
npm outdated         # Show outdated packages
```

## n - version manager

- [n](https://github.com/tj/n)
- [n-install](https://github.com/mklement0/n-install)

Install:

```
curl -L https://git.io/n-install | bash
```

Commands:

```bash
n                    # Output versions installed
n <version>          # Install or activate node <version>
n rm <version ...>   # Remove the given version(s)
n prune              # Remove all versions except the current version
```

## pm2

```bash
pm2 start apps.yml                  # load all apps defined in apps.yml
pm2 save                            # save process list
pm2 reload apps.yml [--update-env]  # reload all apps

pm2 list              # list all processes
pm2 monit             # monitor all processes
pm2 describe 0        # display all information about a specific process

pm2 logs [app]        # display logs
pm2 reset [process]   # reset meta data (restarted time...)
```

- [Update pm2](http://pm2.keymetrics.io/docs/usage/update-pm2/)

```bash
pm2 save
npm install -g pm2
pm2 update
```

## create-react-app

- [Advanced Configuration](https://github.com/facebookincubator/create-react-app/blob/master/packages/react-scripts/template/README.md#advanced-configuration)
- `.env` file:

```
PORT=12345
GENERATE_SOURCEMAP=false
PUBLIC_URL=.               # Build as a local project/file
```
