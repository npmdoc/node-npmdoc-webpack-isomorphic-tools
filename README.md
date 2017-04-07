# api documentation for  [webpack-isomorphic-tools (v3.0.2)](https://github.com/halt-hammerzeit/webpack-isomorphic-tools#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-webpack-isomorphic-tools.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-webpack-isomorphic-tools) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-webpack-isomorphic-tools.svg)](https://travis-ci.org/npmdoc/node-npmdoc-webpack-isomorphic-tools)
#### Transforms CSS-alike text into a React style JSON object

[![NPM](https://nodei.co/npm/webpack-isomorphic-tools.png?downloads=true)](https://www.npmjs.com/package/webpack-isomorphic-tools)

[![apidoc](https://npmdoc.github.io/node-npmdoc-webpack-isomorphic-tools/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-webpack-isomorphic-tools_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-webpack-isomorphic-tools/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-webpack-isomorphic-tools/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-webpack-isomorphic-tools/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Halt Hammerzeit",
        "email": "halt.hammerzeit.at@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/halt-hammerzeit/webpack-isomorphic-tools/issues"
    },
    "dependencies": {
        "babel-runtime": "^6.6.1",
        "colors": "^1.1.2",
        "fs-extra": "^0.30.0",
        "require-hacker": "^3.0.0",
        "sync-request": "^3.0.1",
        "uglify-js": "^2.7.0"
    },
    "description": "Transforms CSS-alike text into a React style JSON object",
    "devDependencies": {
        "babel-cli": "^6.10.1",
        "babel-core": "^6.10.4",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-plugin-transform-runtime": "^6.6.0",
        "babel-preset-es2015": "^6.6.0",
        "babel-preset-stage-0": "^6.5.0",
        "chai": "^3.5.0",
        "coveralls": "^2.11.11",
        "istanbul": "^1.1.0-alpha.1",
        "json-loader": "^0.5.4",
        "minimist": "^1.2.0",
        "mocha": "^2.5.3",
        "npm-run-all": "^2.3.0",
        "rimraf": "^2.5.3"
    },
    "directories": {},
    "dist": {
        "shasum": "565cbb02af873a8924e826dda460ab6b86b87f53",
        "tarball": "https://registry.npmjs.org/webpack-isomorphic-tools/-/webpack-isomorphic-tools-3.0.2.tgz"
    },
    "gitHead": "28fa6897a288f9705bf3f361fe00838cd4fd861e",
    "homepage": "https://github.com/halt-hammerzeit/webpack-isomorphic-tools#readme",
    "keywords": [
        "react",
        "style",
        "inline",
        "css"
    ],
    "license": "MIT",
    "main": "babel-transpiled-modules/index.js",
    "maintainers": [
        {
            "name": "halt-hammerzeit",
            "email": "halt.hammerzeit.at@gmail.com"
        }
    ],
    "name": "webpack-isomorphic-tools",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/halt-hammerzeit/webpack-isomorphic-tools.git"
    },
    "scripts": {
        "build": "npm-run-all clean-for-build build-modules",
        "build-modules": "babel ./source --out-dir ./babel-transpiled-modules --source-maps",
        "clean-for-build": "rimraf ./babel-transpiled-modules/**/*",
        "prepublish": "npm-run-all build test",
        "test": "mocha --compilers js:babel-core/register --colors --bail --reporter spec test/ --recursive",
        "test-coverage": "istanbul cover node_modules/mocha/bin/_mocha -- --compilers js:babel-core/register --colors --reporter dot test/ --recursive",
        "test-travis": "istanbul cover node_modules/mocha/bin/_mocha --report lcovonly -- --compilers js:babel-core/register --colors --reporter spec test/ --recursive"
    },
    "version": "3.0.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module webpack-isomorphic-tools](#apidoc.module.webpack-isomorphic-tools)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.</span>plugin (options)](#apidoc.element.webpack-isomorphic-tools.plugin)
1.  object <span class="apidocSignatureSpan">webpack-isomorphic-tools.</span>common
1.  object <span class="apidocSignatureSpan">webpack-isomorphic-tools.</span>helpers
1.  object <span class="apidocSignatureSpan">webpack-isomorphic-tools.</span>plugin.prototype

#### [module webpack-isomorphic-tools.common](#apidoc.module.webpack-isomorphic-tools.common)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.common.</span>alias_hook (path, module, project_path, aliases, log)](#apidoc.element.webpack-isomorphic-tools.common.alias_hook)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.common.</span>default_webpack_assets ()](#apidoc.element.webpack-isomorphic-tools.common.default_webpack_assets)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.common.</span>is_global_path (path)](#apidoc.element.webpack-isomorphic-tools.common.is_global_path)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.common.</span>is_package_path (path)](#apidoc.element.webpack-isomorphic-tools.common.is_package_path)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.common.</span>is_relative_path (path)](#apidoc.element.webpack-isomorphic-tools.common.is_relative_path)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.common.</span>normalize_asset_path (global_asset_path, project_path)](#apidoc.element.webpack-isomorphic-tools.common.normalize_asset_path)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.common.</span>normalize_options (options)](#apidoc.element.webpack-isomorphic-tools.common.normalize_options)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.common.</span>uniform_path (asset_path)](#apidoc.element.webpack-isomorphic-tools.common.uniform_path)
1.  object <span class="apidocSignatureSpan">webpack-isomorphic-tools.common.</span>verbosity_levels

#### [module webpack-isomorphic-tools.helpers](#apidoc.module.webpack-isomorphic-tools.helpers)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>alias_properties_with_camel_case (object)](#apidoc.element.webpack-isomorphic-tools.helpers.alias_properties_with_camel_case)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>camel_case (string)](#apidoc.element.webpack-isomorphic-tools.helpers.camel_case)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>clone (object)](#apidoc.element.webpack-isomorphic-tools.helpers.clone)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>convert_from_camel_case (object)](#apidoc.element.webpack-isomorphic-tools.helpers.convert_from_camel_case)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>ends_with (string, substring)](#apidoc.element.webpack-isomorphic-tools.helpers.ends_with)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>exists (what)](#apidoc.element.webpack-isomorphic-tools.helpers.exists)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>extend ()](#apidoc.element.webpack-isomorphic-tools.helpers.extend)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>is_blank (text)](#apidoc.element.webpack-isomorphic-tools.helpers.is_blank)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>is_empty (array)](#apidoc.element.webpack-isomorphic-tools.helpers.is_empty)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>is_object (object)](#apidoc.element.webpack-isomorphic-tools.helpers.is_object)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>last (array)](#apidoc.element.webpack-isomorphic-tools.helpers.last)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>merge ()](#apidoc.element.webpack-isomorphic-tools.helpers.merge)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>not_empty (array)](#apidoc.element.webpack-isomorphic-tools.helpers.not_empty)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>repeat (what, times)](#apidoc.element.webpack-isomorphic-tools.helpers.repeat)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>replace_all (where, what, with_what)](#apidoc.element.webpack-isomorphic-tools.helpers.replace_all)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>starts_with (string, substring)](#apidoc.element.webpack-isomorphic-tools.helpers.starts_with)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>zip (a, b)](#apidoc.element.webpack-isomorphic-tools.helpers.zip)

#### [module webpack-isomorphic-tools.plugin](#apidoc.module.webpack-isomorphic-tools.plugin)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.</span>plugin (options)](#apidoc.element.webpack-isomorphic-tools.plugin.plugin)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>cssLoaderParser (module, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.cssLoaderParser)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>cssModulesLoaderParser (module, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.cssModulesLoaderParser)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>css_loader_parser (module, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.css_loader_parser)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>css_modules_loader_parser (module, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.css_modules_loader_parser)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>regular_expression (extensions)](#apidoc.element.webpack-isomorphic-tools.plugin.regular_expression)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>styleLoaderFilter (module, regular_expression, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.styleLoaderFilter)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>styleLoaderPathExtractor (module, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.styleLoaderPathExtractor)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>style_loader_filter (module, regular_expression, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.style_loader_filter)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>style_loader_path_extractor (module, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.style_loader_path_extractor)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>urlLoaderParser (module, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.urlLoaderParser)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>url_loader_parser (module, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.url_loader_parser)

#### [module webpack-isomorphic-tools.plugin.prototype](#apidoc.module.webpack-isomorphic-tools.plugin.prototype)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.prototype.</span>apply (compiler)](#apidoc.element.webpack-isomorphic-tools.plugin.prototype.apply)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.prototype.</span>development (flag)](#apidoc.element.webpack-isomorphic-tools.plugin.prototype.development)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.prototype.</span>regexp (asset_type)](#apidoc.element.webpack-isomorphic-tools.plugin.prototype.regexp)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.prototype.</span>regularExpression (asset_type)](#apidoc.element.webpack-isomorphic-tools.plugin.prototype.regularExpression)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.prototype.</span>regular_expression (asset_type)](#apidoc.element.webpack-isomorphic-tools.plugin.prototype.regular_expression)
1.  [function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.prototype.</span>start_dev_server ()](#apidoc.element.webpack-isomorphic-tools.plugin.prototype.start_dev_server)



# <a name="apidoc.module.webpack-isomorphic-tools"></a>[module webpack-isomorphic-tools](#apidoc.module.webpack-isomorphic-tools)

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.</span>plugin (options)](#apidoc.element.webpack-isomorphic-tools.plugin)
- description and source-code
```javascript
function Webpack_isomorphic_tools_plugin(options) {
	// take the passed in options
	this.options = (0, _helpers.convert_from_camel_case)((0, _helpers.clone)(options));

	// add missing fields, etc
	(0, _common.normalize_options)(this.options);

	// logging
	this.log = new _log2.default('webpack-isomorphic-tools/plugin', { debug: this.options.debug });

	// assets regular expressions (based on extensions).
	// will be used in loaders and in write_assets
	this.regular_expressions = {};

	// for each user defined asset type
	var _iteratorNormalCompletion = true;
	var _didIteratorError = false;
	var _iteratorError = undefined;

	try {
		for (var _iterator = (0, _getIterator3.default)((0, _keys2.default)(this.options.assets)), _step; !(_iteratorNormalCompletion = (
_step = _iterator.next()).done); _iteratorNormalCompletion = true) {
			var asset_type = _step.value;

			var description = this.options.assets[asset_type];

			// create a regular expression for this file extension (or these file extensions)
			this.regular_expressions[asset_type] = description.regular_expression || Webpack_isomorphic_tools_plugin.regular_expression(description
.extensions);
		}
	} catch (err) {
		_didIteratorError = true;
		_iteratorError = err;
	} finally {
		try {
			if (!_iteratorNormalCompletion && _iterator.return) {
				_iterator.return();
			}
		} finally {
			if (_didIteratorError) {
				throw _iteratorError;
			}
		}
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.webpack-isomorphic-tools.common"></a>[module webpack-isomorphic-tools.common](#apidoc.module.webpack-isomorphic-tools.common)

#### <a name="apidoc.element.webpack-isomorphic-tools.common.alias_hook"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.common.</span>alias_hook (path, module, project_path, aliases, log)](#apidoc.element.webpack-isomorphic-tools.common.alias_hook)
- description and source-code
```javascript
function alias_hook(path, module, project_path, aliases, log) {
	// possibly alias the path
	var aliased_path = alias(path, aliases);

	// return if an alias not found
	if (!aliased_path) {
		return;
	}

	// if an alias is found, require() the correct path
	log.debug('require("' + path + '") was called and an alias was found, so aliasing to module path "' + aliased_path + '"');

	// resolve the path to a real filesystem path (resolves 'npm link', etc)
	var global_path = _requireHacker2.default.resolve(aliased_path, module);
	log.debug(' resolved the path for the aliased module to ' + global_path);

	return global_path;

	// const result = require(global_path)
	// // log.debug(' the path was found')

	// return require_hacker.to_javascript_module_source(result)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.common.default_webpack_assets"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.common.</span>default_webpack_assets ()](#apidoc.element.webpack-isomorphic-tools.common.default_webpack_assets)
- description and source-code
```javascript
function default_webpack_assets() {
	var webpack_assets = {
		javascript: {},
		styles: {},
		assets: {}
	};

	return webpack_assets;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.common.is_global_path"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.common.</span>is_global_path (path)](#apidoc.element.webpack-isomorphic-tools.common.is_global_path)
- description and source-code
```javascript
function is_global_path(path) {
	return (0, _helpers.starts_with)(path, '/') || path.indexOf(':') > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.common.is_package_path"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.common.</span>is_package_path (path)](#apidoc.element.webpack-isomorphic-tools.common.is_package_path)
- description and source-code
```javascript
function is_package_path(path) {
	return !is_relative_path(path) && !is_global_path(path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.common.is_relative_path"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.common.</span>is_relative_path (path)](#apidoc.element.webpack-isomorphic-tools.common.is_relative_path)
- description and source-code
```javascript
function is_relative_path(path) {
	return (0, _helpers.starts_with)(path, './') || (0, _helpers.starts_with)(path, '../');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.common.normalize_asset_path"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.common.</span>normalize_asset_path (global_asset_path, project_path)](#apidoc.element.webpack-isomorphic-tools.common.normalize_asset_path)
- description and source-code
```javascript
function normalize_asset_path(global_asset_path, project_path) {
	// // if this path is outside project folder,
	// // return it as a global path
	// if (!starts_with(global_asset_path, project_path + path.sep))
	// {
	// 	return global_asset_path
	// }

	// this path is inside project folder,
	// convert it to a relative path

	// asset path relative to the project folder
	var asset_path = _path2.default.relative(project_path, global_asset_path);

	// for Windows:
	//
	// convert Node.js path to a correct Webpack path
	asset_path = uniform_path(asset_path);

	return asset_path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.common.normalize_options"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.common.</span>normalize_options (options)](#apidoc.element.webpack-isomorphic-tools.common.normalize_options)
- description and source-code
```javascript
function normalize_options(options) {
	// parameters check
	var _iteratorNormalCompletion = true;
	var _didIteratorError = false;
	var _iteratorError = undefined;

	try {
		for (var _iterator = (0, _getIterator3.default)((0, _keys2.default)(options)), _step; !(_iteratorNormalCompletion = (_step = _iterator
.next()).done); _iteratorNormalCompletion = true) {
			var _key = _step.value;

			switch (_key) {
				case 'assets':
					if (!(0, _helpers.is_object)(options[_key])) {
						throw new Error('"' + _key + '" configuration parameter must be ' + 'an object');
					}
					break;

				case 'debug':
					if (typeof options[_key] !== 'boolean') {
						throw new Error('"' + _key + '" configuration parameter must be ' + 'a boolean');
					}
					break;

				case 'verbose':
					if (typeof options[_key] !== 'boolean') {
						throw new Error('"' + _key + '" configuration parameter must be ' + 'a boolean');
					}
					// Legacy 'verbose' option is converted to 'verbosity'
					console.log('[webpack-isomorphic-tools] WARNING: 'verbose' option is now called 'verbosity'');
					if (options.verbose) {
						options.verbosity = verbosity_levels.webpack_stats_for_each_build;
					}
					delete options.verbose;
					break;

				case 'verbosity':
					if (typeof options[_key] !== 'string') {
						throw new Error('"' + _key + '" configuration parameter must be ' + 'a string');
					}
					if ((0, _keys2.default)(verbosity_levels).map(function (key) {
						return verbosity_levels[key];
					}).indexOf(options[_key]) < 0) {
						throw new Error('Unknown "verbosity" passed: ' + options[_key]);
					}
					break;

				case 'port':
					if (typeof options[_key] !== 'number') {
						throw new Error('"' + _key + '" configuration parameter must be ' + 'a number');
					}
					break;

				case 'webpack_assets_file_path':
				case 'webpack_stats_file_path':
					if (typeof options[_key] !== 'string') {
						throw new Error('"' + _key + '" configuration parameter must be ' + 'a string');
					}
					break;

				case 'alias':
					if (!(0, _helpers.is_object)(options[_key])) {
						throw new Error('"' + _key + '" configuration parameter must be ' + 'an object');
					}
					break;

				case 'modules_directories':
					if (!Array.isArray(options[_key])) {
						throw new Error('"' + _key + '" configuration parameter must be ' + 'an array');
					}
					break;

				case 'require_context':
					if (typeof options[_key] !== 'boolean') {
						throw new Error('"' + _key + '" configuration parameter must be ' + 'a boolean');
					}
					// Legacy 'require_context' option is converted to 'patch_require'
					console.log('[webpack-isomorphic-tools] WARNING: 'require_context' option is now called 'patch_require'');
					delete options.require_context;
					options.patch_require = true;
					break;

				case 'patch_require':
					if (typeof options[_key] !== 'boolean') {
						throw new Error('"' + _key + '" configuration parameter must be ' + 'a boolean');
					}
					break;

				default:
					throw new Error('Unknown configuration parameter "' + _key + '"');
			}
		}

		// if no assets specified (for whatever reason), make it an empty array
	} catch (err) {
		_didIteratorError = true;
		_iteratorError = err;
	} finally {
		try {
			if (!_iteratorNormalCompletion && _iterator.return) {
				_iterator.return();
			}
		} finally {
			if (_didIteratorError) {
				throw _iteratorError;
			}
		}
	}

	if (!options.assets) {
		// options.assets = {}
		throw new Error('You must specify "assets" parameter in webpack-isomorphic-tools configuration');
	}

	// webpack-assets.json path, relative to the project base path
	options.webpack_assets_file_path = options.webpack_assets_file_path || 'webpack-assets.json';

	// webpack-stats.json path, relative to the project base path
	options.webpack_stats_file_path = options.webpack_stats_file_path || 'webpack-stats.json';

	// if Webpack aliases are supplied, validate them
	if (options.alias) {
		var _iteratorNormalCompletion2 = true;
		var _didIteratorError2 = false;
		var _iteratorError2 = undefined;

		try {
			for ( ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.common.uniform_path"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.common.</span>uniform_path (asset_path)](#apidoc.element.webpack-isomorphic-tools.common.uniform_path)
- description and source-code
```javascript
function uniform_path(asset_path) {
	// correct slashes
	asset_path = asset_path.replace(/\\/g, '/');

	// add './' in the beginning if it's missing (for example, in case of Windows)
	if (asset_path.indexOf('.') !== 0) {
		asset_path = './' + asset_path;
	}

	return asset_path;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.webpack-isomorphic-tools.helpers"></a>[module webpack-isomorphic-tools.helpers](#apidoc.module.webpack-isomorphic-tools.helpers)

#### <a name="apidoc.element.webpack-isomorphic-tools.helpers.alias_properties_with_camel_case"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>alias_properties_with_camel_case (object)](#apidoc.element.webpack-isomorphic-tools.helpers.alias_properties_with_camel_case)
- description and source-code
```javascript
function alias_properties_with_camel_case(object) {
	var _iteratorNormalCompletion3 = true;
	var _didIteratorError3 = false;
	var _iteratorError3 = undefined;

	try {
		for (var _iterator3 = (0, _getIterator3.default)((0, _keys2.default)(object).filter(function (key) {
			return !is_private_property(key);
		})), _step3; !(_iteratorNormalCompletion3 = (_step3 = _iterator3.next()).done); _iteratorNormalCompletion3 = true) {
			var key = _step3.value;

			object[camel_case(key)] = object[key];
		}
	} catch (err) {
		_didIteratorError3 = true;
		_iteratorError3 = err;
	} finally {
		try {
			if (!_iteratorNormalCompletion3 && _iterator3.return) {
				_iterator3.return();
			}
		} finally {
			if (_didIteratorError3) {
				throw _iteratorError3;
			}
		}
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.helpers.camel_case"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>camel_case (string)](#apidoc.element.webpack-isomorphic-tools.helpers.camel_case)
- description and source-code
```javascript
function camel_case(string) {
	var nameParts = string.split('_');
	return nameParts.slice(1).reduce(function (reduced, current) {
		return reduced + current.charAt(0).toUpperCase() + current.slice(1);
	}, nameParts[0]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.helpers.clone"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>clone (object)](#apidoc.element.webpack-isomorphic-tools.helpers.clone)
- description and source-code
```javascript
function clone(object) {
	if (is_object(object)) {
		return merge({}, object);
	} else if (Array.isArray(object)) {
		return object.map(function (x) {
			return clone(x);
		});
	} else {
		return object;
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.helpers.convert_from_camel_case"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>convert_from_camel_case (object)](#apidoc.element.webpack-isomorphic-tools.helpers.convert_from_camel_case)
- description and source-code
```javascript
function convert_from_camel_case(object) {
	var _iteratorNormalCompletion2 = true;
	var _didIteratorError2 = false;
	var _iteratorError2 = undefined;

	try {
		for (var _iterator2 = (0, _getIterator3.default)((0, _keys2.default)(object)), _step2; !(_iteratorNormalCompletion2 = (_step2 =
_iterator2.next()).done); _iteratorNormalCompletion2 = true) {
			var key = _step2.value;

			if (/[A-Z]/.test(key)) {
				var lo_dashed_key = key.replace(/([A-Z])/g, function (match, group_1) {
					return '_' + group_1.toLowerCase();
				});

				if (!exists(object[lo_dashed_key])) {
					object[lo_dashed_key] = object[key];
					delete object[key];
				}
			}
		}
	} catch (err) {
		_didIteratorError2 = true;
		_iteratorError2 = err;
	} finally {
		try {
			if (!_iteratorNormalCompletion2 && _iterator2.return) {
				_iterator2.return();
			}
		} finally {
			if (_didIteratorError2) {
				throw _iteratorError2;
			}
		}
	}

	return object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.helpers.ends_with"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>ends_with (string, substring)](#apidoc.element.webpack-isomorphic-tools.helpers.ends_with)
- description and source-code
```javascript
function ends_with(string, substring) {
	var i = string.length;
	var j = substring.length;

	if (j > i) {
		return false;
	}

	while (j > 0) {
		i--;
		j--;

		if (string[i] !== substring[j]) {
			return false;
		}
	}

	return true;

	// const index = string.lastIndexOf(substring)
	// return index >= 0 && index === string.length - substring.length
}
```
- example usage
```shell
...
  "name": "./assets/images/husky.jpg",
  "source": "module.exports = __webpack_public_path__ + \"9059f094ddb49c2b0fa6a254a6ebf2ad.jpg\""
}
'''

Therefore, in this simple case, in 'webpack-isomorphic-tools' configuration file we create an "images" asset type with extension
 "jpg" and these parameters:

* the 'filter' function would be 'module => module.name.ends_with('.jpg')' (and it's the default 'filter' if no 'filter' is specified
)
* the 'path' parser function would be 'module => module.name' (and it's the default 'path' parser if no 'path' parser is specified
)
* the 'parser' function would be 'module => module.source' (and it's the default 'parser' if no 'parser' is specified)

When the javascript 'source' code returned by this 'parser' function gets compiled by 'webpack-isomorphic-tools' it will yeild a
 valid CommonJS javascript module which will return the URL for this image, resulting in the following piece of 'webpack-assets.
json':

'''
{
...
```

#### <a name="apidoc.element.webpack-isomorphic-tools.helpers.exists"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>exists (what)](#apidoc.element.webpack-isomorphic-tools.helpers.exists)
- description and source-code
```javascript
function exists(what) {
	return typeof what !== 'undefined';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.helpers.extend"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>extend ()](#apidoc.element.webpack-isomorphic-tools.helpers.extend)
- description and source-code
```javascript
function extend() {
	for (var _len = arguments.length, objects = Array(_len), _key = 0; _key < _len; _key++) {
		objects[_key] = arguments[_key];
	}

	objects = objects.filter(function (x) {
		return exists(x);
	});

	if (objects.length === 0) {
		return;
	}

	if (objects.length === 1) {
		return objects[0];
	}

	var to = objects[0];
	var from = objects[1];

	if (objects.length > 2) {
		var _last = objects.pop();
		var intermediary_result = extend.apply(this, objects);
		return extend(intermediary_result, _last);
	}

	var _iteratorNormalCompletion = true;
	var _didIteratorError = false;
	var _iteratorError = undefined;

	try {
		for (var _iterator = (0, _getIterator3.default)((0, _keys2.default)(from)), _step; !(_iteratorNormalCompletion = (_step = _iterator
.next()).done); _iteratorNormalCompletion = true) {
			var key = _step.value;

			if (is_object(from[key])) {
				if (!is_object(to[key])) {
					to[key] = {};
				}

				extend(to[key], from[key]);
			} else if (Array.isArray(from[key])) {
				if (!Array.isArray(to[key])) {
					to[key] = [];
				}

				to[key] = to[key].concat(clone(from[key]));
			} else {
				to[key] = from[key];
			}
		}
	} catch (err) {
		_didIteratorError = true;
		_iteratorError = err;
	} finally {
		try {
			if (!_iteratorNormalCompletion && _iterator.return) {
				_iterator.return();
			}
		} finally {
			if (_didIteratorError) {
				throw _iteratorError;
			}
		}
	}

	return to;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.helpers.is_blank"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>is_blank (text)](#apidoc.element.webpack-isomorphic-tools.helpers.is_blank)
- description and source-code
```javascript
function is_blank(text) {
	return !exists(text) || !text.replace(/\s/g, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.helpers.is_empty"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>is_empty (array)](#apidoc.element.webpack-isomorphic-tools.helpers.is_empty)
- description and source-code
```javascript
function is_empty(array) {
	return array.length === 0;
}
```
- example usage
```shell
...

{/* styles (will be present only in production with webpack extract text plugin) */}
{Object.keys(assets.styles).map((style, i) =>
  <link href={assets.styles[style]} key={i} media="screen, projection"
        rel="stylesheet" type="text/css"/>)}

{/* resolves the initial style flash (flicker) on page load in development mode */}
{ Object.keys(assets.styles).is_empty() ? <style dangerouslySetInnerHTML={{__html: require('../assets/styles/main_style.css')}}/> :
null }
        </head>

        <body>
{/* image requiring demonstration */}
<img src={picture}/>

{/* rendered React page */}
...
```

#### <a name="apidoc.element.webpack-isomorphic-tools.helpers.is_object"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>is_object (object)](#apidoc.element.webpack-isomorphic-tools.helpers.is_object)
- description and source-code
```javascript
function is_object(object) {
	return exists(object) && object !== null && object.constructor === object_constructor;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.helpers.last"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>last (array)](#apidoc.element.webpack-isomorphic-tools.helpers.last)
- description and source-code
```javascript
function last(array) {
	return array[array.length - 1];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.helpers.merge"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>merge ()](#apidoc.element.webpack-isomorphic-tools.helpers.merge)
- description and source-code
```javascript
function merge() {
	var parameters = Array.prototype.slice.call(arguments, 0);
	parameters.unshift({});
	return extend.apply(this, parameters);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.helpers.not_empty"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>not_empty (array)](#apidoc.element.webpack-isomorphic-tools.helpers.not_empty)
- description and source-code
```javascript
function not_empty(array) {
	return array.length > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.helpers.repeat"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>repeat (what, times)](#apidoc.element.webpack-isomorphic-tools.helpers.repeat)
- description and source-code
```javascript
function repeat(what, times) {
	var result = '';
	while (times > 0) {
		result += what;
		times--;
	}
	return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.helpers.replace_all"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>replace_all (where, what, with_what)](#apidoc.element.webpack-isomorphic-tools.helpers.replace_all)
- description and source-code
```javascript
function replace_all(where, what, with_what) {
	var regexp = new RegExp(escape_regexp(what), 'g');
	return where.replace(regexp, with_what);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.helpers.starts_with"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>starts_with (string, substring)](#apidoc.element.webpack-isomorphic-tools.helpers.starts_with)
- description and source-code
```javascript
function starts_with(string, substring) {
	var j = substring.length;

	if (j > string.length) {
		return false;
	}

	while (j > 0) {
		j--;

		if (string[j] !== substring[j]) {
			return false;
		}
	}

	return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.helpers.zip"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.helpers.</span>zip (a, b)](#apidoc.element.webpack-isomorphic-tools.helpers.zip)
- description and source-code
```javascript
function zip(a, b) {
	return a.map(function (_, index) {
		return [a[index], b[index]];
	});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.webpack-isomorphic-tools.plugin"></a>[module webpack-isomorphic-tools.plugin](#apidoc.module.webpack-isomorphic-tools.plugin)

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.plugin"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.</span>plugin (options)](#apidoc.element.webpack-isomorphic-tools.plugin.plugin)
- description and source-code
```javascript
function Webpack_isomorphic_tools_plugin(options) {
	// take the passed in options
	this.options = (0, _helpers.convert_from_camel_case)((0, _helpers.clone)(options));

	// add missing fields, etc
	(0, _common.normalize_options)(this.options);

	// logging
	this.log = new _log2.default('webpack-isomorphic-tools/plugin', { debug: this.options.debug });

	// assets regular expressions (based on extensions).
	// will be used in loaders and in write_assets
	this.regular_expressions = {};

	// for each user defined asset type
	var _iteratorNormalCompletion = true;
	var _didIteratorError = false;
	var _iteratorError = undefined;

	try {
		for (var _iterator = (0, _getIterator3.default)((0, _keys2.default)(this.options.assets)), _step; !(_iteratorNormalCompletion = (
_step = _iterator.next()).done); _iteratorNormalCompletion = true) {
			var asset_type = _step.value;

			var description = this.options.assets[asset_type];

			// create a regular expression for this file extension (or these file extensions)
			this.regular_expressions[asset_type] = description.regular_expression || Webpack_isomorphic_tools_plugin.regular_expression(description
.extensions);
		}
	} catch (err) {
		_didIteratorError = true;
		_iteratorError = err;
	} finally {
		try {
			if (!_iteratorNormalCompletion && _iterator.return) {
				_iterator.return();
			}
		} finally {
			if (_didIteratorError) {
				throw _iteratorError;
			}
		}
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.cssLoaderParser"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>cssLoaderParser (module, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.cssLoaderParser)
- description and source-code
```javascript
cssLoaderParser = function (module, options, log) {
	return module.source + '\n module.exports = module.exports.toString();';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.cssModulesLoaderParser"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>cssModulesLoaderParser (module, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.cssModulesLoaderParser)
- description and source-code
```javascript
cssModulesLoaderParser = function (module, options, log) {
	return module.source + '\n module.exports = exports.locals || {}; module.exports._style = exports.toString();';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.css_loader_parser"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>css_loader_parser (module, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.css_loader_parser)
- description and source-code
```javascript
css_loader_parser = function (module, options, log) {
	return module.source + '\n module.exports = module.exports.toString();';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.css_modules_loader_parser"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>css_modules_loader_parser (module, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.css_modules_loader_parser)
- description and source-code
```javascript
css_modules_loader_parser = function (module, options, log) {
	return module.source + '\n module.exports = exports.locals || {}; module.exports._style = exports.toString();';
}
```
- example usage
```shell
...
// Basically takes 'module.source' and modifies its 'module.exports' a little.
parser: function(module, options, log)
{
  if (options.development)
  {
    // In development mode it adds an extra '_style' entry
    // to the CSS style class name map, containing the CSS text
    return WebpackIsomorphicToolsPlugin.css_modules_loader_parser(module, options, log);
  }

  // In production mode there's Webpack Extract Text Plugin
  // which extracts all CSS text away, so there's
  // only CSS style class name map left.
  return module.source
}
...
```

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.regular_expression"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>regular_expression (extensions)](#apidoc.element.webpack-isomorphic-tools.plugin.regular_expression)
- description and source-code
```javascript
regular_expression = function (extensions) {
	if (!Array.isArray(extensions)) {
		throw new Error('You were expected to pass a list of extensions (an array). Instead got: ' + extensions + '. Maybe you were looking
 for the instance method istead of the class method of this plugin?');
	}

	var matcher = void 0;
	if (extensions.length > 1) {
		matcher = '(' + extensions.join('|') + ')';
	} else {
		matcher = extensions;
	}

	return new RegExp('\\.' + matcher + '$');
}
```
- example usage
```shell
...

module:
{
  loaders:
  [
    ...,
    {
      test: webpack_isomorphic_tools_plugin.regular_expression('images'),
      loader: 'url-loader?limit=10240', // any image below or equal to 10K will be converted to inline base64 instead
    }
  ]
},

plugins:
[
...
```

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.styleLoaderFilter"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>styleLoaderFilter (module, regular_expression, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.styleLoaderFilter)
- description and source-code
```javascript
styleLoaderFilter = function (module, regular_expression, options, log) {
	var css_loader = module.name.split('!')[0];
	return regular_expression.test(module.name) && (
	// The paths below have the form of "/~/css-loader"
	// and not the form of "./~/css-loader"
	// because in some (non-standard) cases
	// Webpack project context can be set
	// not to project root folder.
	//
	// For a discussion see:
	// https://github.com/halt-hammerzeit/webpack-isomorphic-tools/pull/68
	// (there the 'context' is set to the "${project_root}/src" folder
	//  so that the asset paths in 'webpack-assets.json' wouldn't
	//  contain the "./src" prefix and therefore they will be found
	//  when require()d from code in "./target"
	//  which is compiled with Babel from the "./src" folder)
	//
	// I personally don't compile sources on the server side,
	// so I haven't thought of better ways of doing all that.
	//
	css_loader.indexOf('/~/css-loader') > 0 || css_loader.indexOf('/~/.npminstall/css-loader') > 0 || css_loader.indexOf('/~/.store
/css-loader') > 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.styleLoaderPathExtractor"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>styleLoaderPathExtractor (module, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.styleLoaderPathExtractor)
- description and source-code
```javascript
styleLoaderPathExtractor = function (module, options, log) {
	return module.name.slice(module.name.lastIndexOf('!') + 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.style_loader_filter"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>style_loader_filter (module, regular_expression, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.style_loader_filter)
- description and source-code
```javascript
style_loader_filter = function (module, regular_expression, options, log) {
	var css_loader = module.name.split('!')[0];
	return regular_expression.test(module.name) && (
	// The paths below have the form of "/~/css-loader"
	// and not the form of "./~/css-loader"
	// because in some (non-standard) cases
	// Webpack project context can be set
	// not to project root folder.
	//
	// For a discussion see:
	// https://github.com/halt-hammerzeit/webpack-isomorphic-tools/pull/68
	// (there the 'context' is set to the "${project_root}/src" folder
	//  so that the asset paths in 'webpack-assets.json' wouldn't
	//  contain the "./src" prefix and therefore they will be found
	//  when require()d from code in "./target"
	//  which is compiled with Babel from the "./src" folder)
	//
	// I personally don't compile sources on the server side,
	// so I haven't thought of better ways of doing all that.
	//
	css_loader.indexOf('/~/css-loader') > 0 || css_loader.indexOf('/~/.npminstall/css-loader') > 0 || css_loader.indexOf('/~/.store
/css-loader') > 0);
}
```
- example usage
```shell
...
  //
  // The 'module's containing CSS text are
  // the ones loaded with Webpack "css-loader".
  // (which have kinda weird 'module.name')
  //
  // Therefore using a non-default 'filter' function here.
  //
  return webpack_isomorphic_tools_plugin.style_loader_filter(module, regular_expression, options, log)
}

// In production mode there will be no CSS text at all
// because all styles will be extracted by Webpack Extract Text Plugin
// into a .css file (as per Webpack configuration).
//
// Therefore in production mode 'filter' function always returns non-'true'.
...
```

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.style_loader_path_extractor"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>style_loader_path_extractor (module, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.style_loader_path_extractor)
- description and source-code
```javascript
style_loader_path_extractor = function (module, options, log) {
	return module.name.slice(module.name.lastIndexOf('!') + 1);
}
```
- example usage
```shell
...
  if (options.development)
  {
    // In development mode there's Webpack "style-loader",
    // so 'module.name's of the 'module's created by Webpack "css-loader"
    // (those picked by the 'filter' function above)
    // will be kinda weird, and this path extractor extracts
    // the correct asset paths from these kinda weird 'module.name's
    return WebpackIsomorphicToolsPlugin.style_loader_path_extractor(module, options, log);
  }

  // in production mode there's no Webpack "style-loader",
  // so 'module.name's will be equal to correct asset paths
  return module.name
},
...
```

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.urlLoaderParser"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>urlLoaderParser (module, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.urlLoaderParser)
- description and source-code
```javascript
urlLoaderParser = function (module, options, log) {
	return module.source;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.url_loader_parser"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.</span>url_loader_parser (module, options, log)](#apidoc.element.webpack-isomorphic-tools.plugin.url_loader_parser)
- description and source-code
```javascript
url_loader_parser = function (module, options, log) {
	return module.source;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.webpack-isomorphic-tools.plugin.prototype"></a>[module webpack-isomorphic-tools.plugin.prototype](#apidoc.module.webpack-isomorphic-tools.plugin.prototype)

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.prototype.apply"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.prototype.</span>apply (compiler)](#apidoc.element.webpack-isomorphic-tools.plugin.prototype.apply)
- description and source-code
```javascript
apply = function (compiler) {
	// start HTTP service in development mode
	// https://github.com/halt-hammerzeit/webpack-isomorphic-tools/issues/92
	//
	// ('.apply()' is only called once, so can start the dev server here)
	//
	if (this.options.development && this.options.port) {
		this.start_dev_server();
	}

	// Webpack configuration
	var webpack_configuration = compiler.options;

	// validate webpack configuration
	if (!webpack_configuration.context) {
		throw new Error('You must specify ".context" in your webpack configuration');
	}

	// project base path, required to output webpack-assets.json
	this.options.project_path = webpack_configuration.context;

	// resolve webpack-assets.json file path
	var webpack_assets_path = _path2.default.resolve(this.options.project_path, this.options.webpack_assets_file_path);

	// resolve webpack-stats.json file path
	var webpack_stats_path = _path2.default.resolve(this.options.project_path, this.options.webpack_stats_file_path);

	// selfie
	var plugin = this;

	// when all is done
	// https://github.com/webpack/docs/wiki/plugins
	compiler.plugin('done', function (stats) {
		plugin.log.debug('------------------- Started -------------------');

		var json = stats.toJson({
			context: webpack_configuration.context
		});

		// output some info to the console if in development mode
		if (plugin.options.development && plugin.options.verbosity !== _common.verbosity_levels.no_webpack_stats) {
			// outputs stats info to the console
			// (only needed in development mode)
			(0, _notifyStats2.default)(stats, json, plugin.options.verbosity === _common.verbosity_levels.webpack_stats_for_each_build);
		}

		// assets base path (on disk or on the network)
		//
		// (first search for the 'devServer.publicPath' setting,
		//  then fallback to the generic 'publicPath')
		//
		// (using 'publicPath' from webpack stats here
		//  as opposed to 'webpack_configuration.output.publicPath'
		//  because it is processed by webpack replacing things like '[hash]')
		//
		var assets_base_url = process.env.NODE_ENV !== 'production' && webpack_configuration.devServer && webpack_configuration.devServer
.publicPath ? webpack_configuration.devServer.publicPath : json.publicPath;

		// serve webpack assets from RAM rather than from disk
		var serve_assets_from_memory = plugin.options.development && plugin.options.port;

		// write webpack-assets.json with assets info
		// and cache them in plugin instance
		// for later serving from HTTP service
		plugin.assets = (0, _writeAssets2.default)(json, {
			development: plugin.options.development,
			debug: plugin.options.debug,
			assets: plugin.options.assets,
			alias: plugin.options.alias,
			project_path: plugin.options.project_path,
			assets_base_url: assets_base_url,
			webpack_assets_path: webpack_assets_path,
			webpack_stats_path: webpack_stats_path,
			output: (0, _common.default_webpack_assets)(),
			output_to_a_file: !serve_assets_from_memory,
			regular_expressions: plugin.regular_expressions
		}, plugin.log);

		plugin.log.debug('------------------- Finished -------------------');
	});
}
```
- example usage
```shell
...
	}

	var to = objects[0];
	var from = objects[1];

	if (objects.length > 2) {
		var _last = objects.pop();
		var intermediary_result = extend.apply(this, objects);
		return extend(intermediary_result, _last);
	}

	var _iteratorNormalCompletion = true;
	var _didIteratorError = false;
	var _iteratorError = undefined;
...
```

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.prototype.development"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.prototype.</span>development (flag)](#apidoc.element.webpack-isomorphic-tools.plugin.prototype.development)
- description and source-code
```javascript
development = function (flag) {
	// set development mode flag
	this.options.development = (0, _helpers.exists)(flag) ? flag : true;

	if (this.options.development) {
		this.log.debug('entering development mode');
	} else {
		this.log.debug('entering production mode');
	}

	// allows method chaining
	return this;
}
```
- example usage
```shell
...

var webpack_isomorphic_tools_plugin =
// webpack-isomorphic-tools settings reside in a separate .js file
// (because they will be used in the web server code too).
new Webpack_isomorphic_tools_plugin(require('./webpack-isomorphic-tools-configuration'))
// also enter development mode since it's a development webpack configuration
// (see below for explanation)
.development()

// usual Webpack configuration
module.exports =
{
context: '(required) your project path here',

module:
...
```

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.prototype.regexp"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.prototype.</span>regexp (asset_type)](#apidoc.element.webpack-isomorphic-tools.plugin.prototype.regexp)
- description and source-code
```javascript
regexp = function (asset_type) {
	if (!(0, _helpers.exists)(this.regular_expressions[asset_type])) {
		throw new Error('There\'s no asset type "' + asset_type + '" defined in webpack-isomorphic-tools configuration. Perhaps you didn\'t spell it correctly.');
	}

	return this.regular_expressions[asset_type];
}
```
- example usage
```shell
...

(Webpack plugin instance only)

Is it development mode or is it production mode? By default it's production mode. But if you're instantiating 'webpack-isomorphic
-tools/plugin' for use in Webpack development configuration, then you should call this method to enable asset hot reloading (and
 disable asset caching), and optinally to run its own "dev server" utility (see 'port' configuration setting). It should be called
 right after the constructor.

#### .regular_expression(asset_type)

(aka '.regexp(asset_type)')

(Webpack plugin instance)

Returns the regular expression for this asset type (based on this asset type's 'extension' (or 'extensions'))

#### Webpack_isomorphic_tools_plugin.url_loader_parser
...
```

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.prototype.regularExpression"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.prototype.</span>regularExpression (asset_type)](#apidoc.element.webpack-isomorphic-tools.plugin.prototype.regularExpression)
- description and source-code
```javascript
regularExpression = function (asset_type) {
	if (!(0, _helpers.exists)(this.regular_expressions[asset_type])) {
		throw new Error('There\'s no asset type "' + asset_type + '" defined in webpack-isomorphic-tools configuration. Perhaps you didn\'t spell it correctly.');
	}

	return this.regular_expressions[asset_type];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.prototype.regular_expression"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.prototype.</span>regular_expression (asset_type)](#apidoc.element.webpack-isomorphic-tools.plugin.prototype.regular_expression)
- description and source-code
```javascript
regular_expression = function (asset_type) {
	if (!(0, _helpers.exists)(this.regular_expressions[asset_type])) {
		throw new Error('There\'s no asset type "' + asset_type + '" defined in webpack-isomorphic-tools configuration. Perhaps you didn\'t spell it correctly.');
	}

	return this.regular_expressions[asset_type];
}
```
- example usage
```shell
...

module:
{
  loaders:
  [
    ...,
    {
      test: webpack_isomorphic_tools_plugin.regular_expression('images'),
      loader: 'url-loader?limit=10240', // any image below or equal to 10K will be converted to inline base64 instead
    }
  ]
},

plugins:
[
...
```

#### <a name="apidoc.element.webpack-isomorphic-tools.plugin.prototype.start_dev_server"></a>[function <span class="apidocSignatureSpan">webpack-isomorphic-tools.plugin.prototype.</span>start_dev_server ()](#apidoc.element.webpack-isomorphic-tools.plugin.prototype.start_dev_server)
- description and source-code
```javascript
start_dev_server = function () {
	var _this = this;

	var express = require('express');
	var app = express();

	app.get('/', function (request, response) {
		if (!_this.assets) {
			return response.status(404).send('Webpack assets not generated yet');
		}

		response.send(_this.assets);
	});

	app.listen(this.options.port, function () {
		_this.log.info('HTTP service listening on port ' + _this.options.port);
	});
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
