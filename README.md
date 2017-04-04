# api documentation for  [nunjucks (v3.0.0)](https://github.com/mozilla/nunjucks#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-nunjucks.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-nunjucks) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-nunjucks.svg)](https://travis-ci.org/npmdoc/node-npmdoc-nunjucks)
#### A powerful templating engine with inheritance, asynchronous control, and more (jinja2 inspired)

[![NPM](https://nodei.co/npm/nunjucks.png?downloads=true)](https://www.npmjs.com/package/nunjucks)

[![apidoc](https://npmdoc.github.io/node-npmdoc-nunjucks/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-nunjucks_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-nunjucks/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-nunjucks/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-nunjucks/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "James Long",
        "email": "longster@gmail.com"
    },
    "bin": {
        "nunjucks-precompile": "./bin/precompile"
    },
    "browser": "./browser/nunjucks.js",
    "bugs": {
        "url": "https://github.com/mozilla/nunjucks/issues"
    },
    "dependencies": {
        "a-sync-waterfall": "^1.0.0",
        "asap": "^2.0.3",
        "chokidar": "^1.6.0",
        "yargs": "^3.32.0"
    },
    "description": "A powerful templating engine with inheritance, asynchronous control, and more (jinja2 inspired)",
    "devDependencies": {
        "expect.js": "*",
        "express": "4.x",
        "istanbul": "0.3.x",
        "jshint": "2.8.x",
        "mocha": "*",
        "node-libs-browser": "^0.4.3",
        "supertest": "*",
        "uglify-js": "*",
        "webpack": "^1.8.11"
    },
    "directories": {},
    "dist": {
        "shasum": "0a2a8fd2942a3ba04f5ba6684e4f7f7ceaca8305",
        "tarball": "https://registry.npmjs.org/nunjucks/-/nunjucks-3.0.0.tgz"
    },
    "engines": {
        "node": "*"
    },
    "gitHead": "737e4e005cd2a62f1d9e7cd4552b76b21d368930",
    "homepage": "https://github.com/mozilla/nunjucks#readme",
    "keywords": [
        "template",
        "templating"
    ],
    "license": "BSD-2-Clause",
    "main": "index",
    "maintainers": [
        {
            "name": "carljm",
            "email": "carl@oddbird.net"
        },
        {
            "name": "jlongster",
            "email": "longster@gmail.com"
        },
        {
            "name": "samypesse",
            "email": "samypesse@gmail.com"
        },
        {
            "name": "vecmezoni",
            "email": "alexander.inozemtsev@gmail.com"
        }
    ],
    "name": "nunjucks",
    "optionalDependencies": {
        "chokidar": "^1.6.0"
    },
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mozilla/nunjucks.git"
    },
    "scripts": {
        "browserfiles": "./bin/bundle",
        "lint": "jshint .",
        "test": "jshint . && istanbul cover ./node_modules/mocha/bin/_mocha -- -R dot tests"
    },
    "version": "3.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module nunjucks](#apidoc.module.nunjucks)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>Environment ()](#apidoc.element.nunjucks.Environment)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>FileSystemLoader ()](#apidoc.element.nunjucks.FileSystemLoader)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>Loader ()](#apidoc.element.nunjucks.Loader)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>PrecompiledLoader ()](#apidoc.element.nunjucks.PrecompiledLoader)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>Template ()](#apidoc.element.nunjucks.Template)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>compile (src, env, path, eagerCompile)](#apidoc.element.nunjucks.compile)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>compiler.Compiler ()](#apidoc.element.nunjucks.compiler.Compiler)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>configure (templatesPath, opts)](#apidoc.element.nunjucks.configure)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>installJinjaCompat ()](#apidoc.element.nunjucks.installJinjaCompat)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Add ()](#apidoc.element.nunjucks.nodes.Add)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.And ()](#apidoc.element.nunjucks.nodes.And)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Array ()](#apidoc.element.nunjucks.nodes.Array)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.AsyncAll ()](#apidoc.element.nunjucks.nodes.AsyncAll)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.AsyncEach ()](#apidoc.element.nunjucks.nodes.AsyncEach)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.BinOp ()](#apidoc.element.nunjucks.nodes.BinOp)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Block ()](#apidoc.element.nunjucks.nodes.Block)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.CallExtension ()](#apidoc.element.nunjucks.nodes.CallExtension)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.CallExtensionAsync ()](#apidoc.element.nunjucks.nodes.CallExtensionAsync)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Caller ()](#apidoc.element.nunjucks.nodes.Caller)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Capture ()](#apidoc.element.nunjucks.nodes.Capture)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Compare ()](#apidoc.element.nunjucks.nodes.Compare)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.CompareOperand ()](#apidoc.element.nunjucks.nodes.CompareOperand)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Concat ()](#apidoc.element.nunjucks.nodes.Concat)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Dict ()](#apidoc.element.nunjucks.nodes.Dict)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Div ()](#apidoc.element.nunjucks.nodes.Div)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Extends ()](#apidoc.element.nunjucks.nodes.Extends)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Filter ()](#apidoc.element.nunjucks.nodes.Filter)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.FilterAsync ()](#apidoc.element.nunjucks.nodes.FilterAsync)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.FloorDiv ()](#apidoc.element.nunjucks.nodes.FloorDiv)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.For ()](#apidoc.element.nunjucks.nodes.For)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.FromImport ()](#apidoc.element.nunjucks.nodes.FromImport)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.FunCall ()](#apidoc.element.nunjucks.nodes.FunCall)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Group ()](#apidoc.element.nunjucks.nodes.Group)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.If ()](#apidoc.element.nunjucks.nodes.If)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.IfAsync ()](#apidoc.element.nunjucks.nodes.IfAsync)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Import ()](#apidoc.element.nunjucks.nodes.Import)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.In ()](#apidoc.element.nunjucks.nodes.In)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Include ()](#apidoc.element.nunjucks.nodes.Include)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.InlineIf ()](#apidoc.element.nunjucks.nodes.InlineIf)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.KeywordArgs ()](#apidoc.element.nunjucks.nodes.KeywordArgs)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Literal ()](#apidoc.element.nunjucks.nodes.Literal)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.LookupVal ()](#apidoc.element.nunjucks.nodes.LookupVal)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Macro ()](#apidoc.element.nunjucks.nodes.Macro)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Mod ()](#apidoc.element.nunjucks.nodes.Mod)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Mul ()](#apidoc.element.nunjucks.nodes.Mul)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Neg ()](#apidoc.element.nunjucks.nodes.Neg)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Node ()](#apidoc.element.nunjucks.nodes.Node)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.NodeList ()](#apidoc.element.nunjucks.nodes.NodeList)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Not ()](#apidoc.element.nunjucks.nodes.Not)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Or ()](#apidoc.element.nunjucks.nodes.Or)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Output ()](#apidoc.element.nunjucks.nodes.Output)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Pair ()](#apidoc.element.nunjucks.nodes.Pair)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Pos ()](#apidoc.element.nunjucks.nodes.Pos)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Pow ()](#apidoc.element.nunjucks.nodes.Pow)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Root ()](#apidoc.element.nunjucks.nodes.Root)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Set ()](#apidoc.element.nunjucks.nodes.Set)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Sub ()](#apidoc.element.nunjucks.nodes.Sub)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Super ()](#apidoc.element.nunjucks.nodes.Super)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Symbol ()](#apidoc.element.nunjucks.nodes.Symbol)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.TemplateData ()](#apidoc.element.nunjucks.nodes.TemplateData)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Value ()](#apidoc.element.nunjucks.nodes.Value)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>object ()](#apidoc.element.nunjucks.object)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>precompile (input, opts)](#apidoc.element.nunjucks.precompile)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>precompileString (str, opts)](#apidoc.element.nunjucks.precompileString)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>render (name, ctx, cb)](#apidoc.element.nunjucks.render)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>renderString (src, ctx, cb)](#apidoc.element.nunjucks.renderString)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>runtime.Frame ()](#apidoc.element.nunjucks.runtime.Frame)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>runtime.SafeString (val)](#apidoc.element.nunjucks.runtime.SafeString)
1.  object <span class="apidocSignatureSpan"></span>nunjucks
1.  object <span class="apidocSignatureSpan">nunjucks.</span>Environment.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>FileSystemLoader.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>Loader.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>PrecompiledLoader.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>Template.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>compiler
1.  object <span class="apidocSignatureSpan">nunjucks.</span>compiler.Compiler.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>environment
1.  object <span class="apidocSignatureSpan">nunjucks.</span>filters
1.  object <span class="apidocSignatureSpan">nunjucks.</span>lexer
1.  object <span class="apidocSignatureSpan">nunjucks.</span>lib
1.  object <span class="apidocSignatureSpan">nunjucks.</span>loaders
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Add.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.And.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Array.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.AsyncAll.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.AsyncEach.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.BinOp.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Block.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.CallExtension.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.CallExtensionAsync.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Caller.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Capture.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Compare.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.CompareOperand.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Concat.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Dict.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Div.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Extends.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Filter.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.FilterAsync.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.FloorDiv.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.For.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.FromImport.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.FunCall.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Group.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.If.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.IfAsync.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Import.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.In.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Include.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.InlineIf.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.KeywordArgs.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Literal.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.LookupVal.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Macro.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Mod.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Mul.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Neg.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Node.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.NodeList.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Not.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Or.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Output.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Pair.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Pos.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Pow.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Root.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Set.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Sub.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Super.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Symbol.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.TemplateData.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nodes.Value.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>nunjucks_slim
1.  object <span class="apidocSignatureSpan">nunjucks.</span>object.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>parser
1.  object <span class="apidocSignatureSpan">nunjucks.</span>runtime
1.  object <span class="apidocSignatureSpan">nunjucks.</span>runtime.Frame.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>runtime.SafeString.prototype
1.  object <span class="apidocSignatureSpan">nunjucks.</span>transformer
1.  object <span class="apidocSignatureSpan">nunjucks.</span>web_loaders

#### [module nunjucks.Environment](#apidoc.module.nunjucks.Environment)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>Environment ()](#apidoc.element.nunjucks.Environment.Environment)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.</span>extend (name, props)](#apidoc.element.nunjucks.Environment.extend)

#### [module nunjucks.Environment.prototype](#apidoc.module.nunjucks.Environment.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>addExtension (name, extension)](#apidoc.element.nunjucks.Environment.prototype.addExtension)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>addFilter (name, func, async)](#apidoc.element.nunjucks.Environment.prototype.addFilter)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>addGlobal (name, value)](#apidoc.element.nunjucks.Environment.prototype.addGlobal)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>constructor ()](#apidoc.element.nunjucks.Environment.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>express (app)](#apidoc.element.nunjucks.Environment.prototype.express)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>getExtension (name)](#apidoc.element.nunjucks.Environment.prototype.getExtension)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>getFilter (name)](#apidoc.element.nunjucks.Environment.prototype.getFilter)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>getGlobal (name)](#apidoc.element.nunjucks.Environment.prototype.getGlobal)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>getTemplate (name, eagerCompile, parentName, ignoreMissing, cb)](#apidoc.element.nunjucks.Environment.prototype.getTemplate)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>hasExtension (name)](#apidoc.element.nunjucks.Environment.prototype.hasExtension)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>init (loaders, opts)](#apidoc.element.nunjucks.Environment.prototype.init)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>initCache ()](#apidoc.element.nunjucks.Environment.prototype.initCache)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>removeExtension (name)](#apidoc.element.nunjucks.Environment.prototype.removeExtension)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>render (name, ctx, cb)](#apidoc.element.nunjucks.Environment.prototype.render)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>renderString (src, ctx, opts, cb)](#apidoc.element.nunjucks.Environment.prototype.renderString)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>resolveTemplate (loader, parentName, filename)](#apidoc.element.nunjucks.Environment.prototype.resolveTemplate)
1.  [function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>waterfall (tasks, callback, forceAsync)](#apidoc.element.nunjucks.Environment.prototype.waterfall)
1.  string <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>typename

#### [module nunjucks.FileSystemLoader](#apidoc.module.nunjucks.FileSystemLoader)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>FileSystemLoader ()](#apidoc.element.nunjucks.FileSystemLoader.FileSystemLoader)
1.  [function <span class="apidocSignatureSpan">nunjucks.FileSystemLoader.</span>extend (name, props)](#apidoc.element.nunjucks.FileSystemLoader.extend)

#### [module nunjucks.FileSystemLoader.prototype](#apidoc.module.nunjucks.FileSystemLoader.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.FileSystemLoader.prototype.</span>constructor ()](#apidoc.element.nunjucks.FileSystemLoader.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nunjucks.FileSystemLoader.prototype.</span>getSource (name)](#apidoc.element.nunjucks.FileSystemLoader.prototype.getSource)
1.  [function <span class="apidocSignatureSpan">nunjucks.FileSystemLoader.prototype.</span>init (searchPaths, opts)](#apidoc.element.nunjucks.FileSystemLoader.prototype.init)
1.  string <span class="apidocSignatureSpan">nunjucks.FileSystemLoader.prototype.</span>typename

#### [module nunjucks.Loader](#apidoc.module.nunjucks.Loader)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>Loader ()](#apidoc.element.nunjucks.Loader.Loader)
1.  [function <span class="apidocSignatureSpan">nunjucks.Loader.</span>extend (name, props)](#apidoc.element.nunjucks.Loader.extend)

#### [module nunjucks.Loader.prototype](#apidoc.module.nunjucks.Loader.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.Loader.prototype.</span>constructor ()](#apidoc.element.nunjucks.Loader.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nunjucks.Loader.prototype.</span>emit (name)](#apidoc.element.nunjucks.Loader.prototype.emit)
1.  [function <span class="apidocSignatureSpan">nunjucks.Loader.prototype.</span>isRelative (filename)](#apidoc.element.nunjucks.Loader.prototype.isRelative)
1.  [function <span class="apidocSignatureSpan">nunjucks.Loader.prototype.</span>on (name, func)](#apidoc.element.nunjucks.Loader.prototype.on)
1.  [function <span class="apidocSignatureSpan">nunjucks.Loader.prototype.</span>resolve (from, to)](#apidoc.element.nunjucks.Loader.prototype.resolve)
1.  string <span class="apidocSignatureSpan">nunjucks.Loader.prototype.</span>typename

#### [module nunjucks.PrecompiledLoader](#apidoc.module.nunjucks.PrecompiledLoader)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>PrecompiledLoader ()](#apidoc.element.nunjucks.PrecompiledLoader.PrecompiledLoader)
1.  [function <span class="apidocSignatureSpan">nunjucks.PrecompiledLoader.</span>extend (name, props)](#apidoc.element.nunjucks.PrecompiledLoader.extend)

#### [module nunjucks.PrecompiledLoader.prototype](#apidoc.module.nunjucks.PrecompiledLoader.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.PrecompiledLoader.prototype.</span>constructor ()](#apidoc.element.nunjucks.PrecompiledLoader.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nunjucks.PrecompiledLoader.prototype.</span>getSource (name)](#apidoc.element.nunjucks.PrecompiledLoader.prototype.getSource)
1.  [function <span class="apidocSignatureSpan">nunjucks.PrecompiledLoader.prototype.</span>init (compiledTemplates)](#apidoc.element.nunjucks.PrecompiledLoader.prototype.init)
1.  string <span class="apidocSignatureSpan">nunjucks.PrecompiledLoader.prototype.</span>typename

#### [module nunjucks.Template](#apidoc.module.nunjucks.Template)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>Template ()](#apidoc.element.nunjucks.Template.Template)
1.  [function <span class="apidocSignatureSpan">nunjucks.Template.</span>extend (name, props)](#apidoc.element.nunjucks.Template.extend)

#### [module nunjucks.Template.prototype](#apidoc.module.nunjucks.Template.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.Template.prototype.</span>_compile ()](#apidoc.element.nunjucks.Template.prototype._compile)
1.  [function <span class="apidocSignatureSpan">nunjucks.Template.prototype.</span>_getBlocks (props)](#apidoc.element.nunjucks.Template.prototype._getBlocks)
1.  [function <span class="apidocSignatureSpan">nunjucks.Template.prototype.</span>compile ()](#apidoc.element.nunjucks.Template.prototype.compile)
1.  [function <span class="apidocSignatureSpan">nunjucks.Template.prototype.</span>constructor ()](#apidoc.element.nunjucks.Template.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nunjucks.Template.prototype.</span>getExported (ctx, parentFrame, cb)](#apidoc.element.nunjucks.Template.prototype.getExported)
1.  [function <span class="apidocSignatureSpan">nunjucks.Template.prototype.</span>init (src, env, path, eagerCompile)](#apidoc.element.nunjucks.Template.prototype.init)
1.  [function <span class="apidocSignatureSpan">nunjucks.Template.prototype.</span>render (ctx, parentFrame, cb)](#apidoc.element.nunjucks.Template.prototype.render)
1.  string <span class="apidocSignatureSpan">nunjucks.Template.prototype.</span>typename

#### [module nunjucks.compiler](#apidoc.module.nunjucks.compiler)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.</span>Compiler ()](#apidoc.element.nunjucks.compiler.Compiler)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.</span>compile (src, asyncFilters, extensions, name, opts)](#apidoc.element.nunjucks.compiler.compile)

#### [module nunjucks.compiler.Compiler](#apidoc.module.nunjucks.compiler.Compiler)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.</span>Compiler ()](#apidoc.element.nunjucks.compiler.Compiler.Compiler)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.</span>extend (name, props)](#apidoc.element.nunjucks.compiler.Compiler.extend)

#### [module nunjucks.compiler.Compiler.prototype](#apidoc.module.nunjucks.compiler.Compiler.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>_compileAggregate (node, frame, startChar, endChar)](#apidoc.element.nunjucks.compiler.Compiler.prototype._compileAggregate)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>_compileAsyncLoop (node, frame, parallel)](#apidoc.element.nunjucks.compiler.Compiler.prototype._compileAsyncLoop)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>_compileChildren (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype._compileChildren)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>_compileExpression (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype._compileExpression)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>_compileMacro (node)](#apidoc.element.nunjucks.compiler.Compiler.prototype._compileMacro)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>_getNodeName (node)](#apidoc.element.nunjucks.compiler.Compiler.prototype._getNodeName)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>_templateName ()](#apidoc.element.nunjucks.compiler.Compiler.prototype._templateName)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>addScopeLevel ()](#apidoc.element.nunjucks.compiler.Compiler.prototype.addScopeLevel)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>assertType (node)](#apidoc.element.nunjucks.compiler.Compiler.prototype.assertType)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>closeScopeLevels ()](#apidoc.element.nunjucks.compiler.Compiler.prototype.closeScopeLevels)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compile (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compile)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileAdd (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileAdd)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileAnd (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileAnd)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileArray (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileArray)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileAsyncAll (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileAsyncAll)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileAsyncEach (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileAsyncEach)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileBlock (node)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileBlock)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileCallExtension (node, frame, async)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileCallExtension)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileCallExtensionAsync (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileCallExtensionAsync)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileCaller (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileCaller)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileCapture (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileCapture)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileCompare (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileCompare)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileConcat (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileConcat)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileDict (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileDict)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileDiv (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileDiv)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileExtends (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileExtends)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileFilter (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileFilter)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileFilterAsync (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileFilterAsync)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileFloorDiv (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileFloorDiv)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileFor (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileFor)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileFromImport (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileFromImport)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileFunCall (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileFunCall)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileGroup (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileGroup)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileIf (node, frame, async)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileIf)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileIfAsync (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileIfAsync)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileImport (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileImport)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileIn (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileIn)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileInclude (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileInclude)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileInlineIf (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileInlineIf)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileKeywordArgs (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileKeywordArgs)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileLiteral (node)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileLiteral)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileLookupVal (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileLookupVal)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileMacro (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileMacro)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileMod (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileMod)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileMul (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileMul)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileNeg (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileNeg)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileNodeList (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileNodeList)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileNot (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileNot)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileOr (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileOr)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileOutput (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileOutput)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compilePair (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compilePair)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compilePos (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compilePos)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compilePow (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compilePow)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileRoot (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileRoot)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileSet (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileSet)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileSub (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileSub)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileSuper (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileSuper)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileSymbol (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileSymbol)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileTemplateData (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileTemplateData)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>constructor ()](#apidoc.element.nunjucks.compiler.Compiler.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>emit (code)](#apidoc.element.nunjucks.compiler.Compiler.prototype.emit)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>emitFuncBegin (name)](#apidoc.element.nunjucks.compiler.Compiler.prototype.emitFuncBegin)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>emitFuncEnd (noReturn)](#apidoc.element.nunjucks.compiler.Compiler.prototype.emitFuncEnd)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>emitLine (code)](#apidoc.element.nunjucks.compiler.Compiler.prototype.emitLine)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>emitLines ()](#apidoc.element.nunjucks.compiler.Compiler.prototype.emitLines)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>emitLoopBindings (node, arr, i, len)](#apidoc.element.nunjucks.compiler.Compiler.prototype.emitLoopBindings)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>fail (msg, lineno, colno)](#apidoc.element.nunjucks.compiler.Compiler.prototype.fail)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>getCode ()](#apidoc.element.nunjucks.compiler.Compiler.prototype.getCode)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>init (templateName, throwOnUndefined)](#apidoc.element.nunjucks.compiler.Compiler.prototype.init)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>makeCallback (res)](#apidoc.element.nunjucks.compiler.Compiler.prototype.makeCallback)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>popBufferId ()](#apidoc.element.nunjucks.compiler.Compiler.prototype.popBufferId)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>pushBufferId (id)](#apidoc.element.nunjucks.compiler.Compiler.prototype.pushBufferId)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>tmpid ()](#apidoc.element.nunjucks.compiler.Compiler.prototype.tmpid)
1.  [function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>withScopedSyntax (func)](#apidoc.element.nunjucks.compiler.Compiler.prototype.withScopedSyntax)
1.  string <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>typename

#### [module nunjucks.environment](#apidoc.module.nunjucks.environment)
1.  [function <span class="apidocSignatureSpan">nunjucks.environment.</span>Environment ()](#apidoc.element.nunjucks.environment.Environment)
1.  [function <span class="apidocSignatureSpan">nunjucks.environment.</span>Template ()](#apidoc.element.nunjucks.environment.Template)

#### [module nunjucks.filters](#apidoc.module.nunjucks.filters)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>abs (n)](#apidoc.element.nunjucks.filters.abs)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>batch (arr, linecount, fill_with)](#apidoc.element.nunjucks.filters.batch)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>capitalize (str)](#apidoc.element.nunjucks.filters.capitalize)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>center (str, width)](#apidoc.element.nunjucks.filters.center)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>d (val, def, bool)](#apidoc.element.nunjucks.filters.d)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>default (val, def, bool)](#apidoc.element.nunjucks.filters.default)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>dictsort (val, case_sensitive, by)](#apidoc.element.nunjucks.filters.dictsort)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>dump (obj, spaces)](#apidoc.element.nunjucks.filters.dump)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>e (str)](#apidoc.element.nunjucks.filters.e)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>escape (str)](#apidoc.element.nunjucks.filters.escape)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>first (arr)](#apidoc.element.nunjucks.filters.first)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>float (val, def)](#apidoc.element.nunjucks.filters.float)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>groupby (arr, attr)](#apidoc.element.nunjucks.filters.groupby)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>indent (str, width, indentfirst)](#apidoc.element.nunjucks.filters.indent)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>int (val, def)](#apidoc.element.nunjucks.filters.int)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>join (arr, del, attr)](#apidoc.element.nunjucks.filters.join)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>last (arr)](#apidoc.element.nunjucks.filters.last)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>length (val)](#apidoc.element.nunjucks.filters.length)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>list (val)](#apidoc.element.nunjucks.filters.list)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>lower (str)](#apidoc.element.nunjucks.filters.lower)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>nl2br (str)](#apidoc.element.nunjucks.filters.nl2br)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>random (arr)](#apidoc.element.nunjucks.filters.random)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>rejectattr (arr, attr)](#apidoc.element.nunjucks.filters.rejectattr)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>replace (str, old, new_, maxCount)](#apidoc.element.nunjucks.filters.replace)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>reverse (val)](#apidoc.element.nunjucks.filters.reverse)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>round (val, precision, method)](#apidoc.element.nunjucks.filters.round)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>safe (str)](#apidoc.element.nunjucks.filters.safe)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>selectattr (arr, attr)](#apidoc.element.nunjucks.filters.selectattr)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>slice (arr, slices, fillWith)](#apidoc.element.nunjucks.filters.slice)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>sort ()](#apidoc.element.nunjucks.filters.sort)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>string (obj)](#apidoc.element.nunjucks.filters.string)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>striptags (input, preserve_linebreaks)](#apidoc.element.nunjucks.filters.striptags)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>sum (arr, attr, start)](#apidoc.element.nunjucks.filters.sum)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>title (str)](#apidoc.element.nunjucks.filters.title)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>trim (str)](#apidoc.element.nunjucks.filters.trim)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>truncate (input, length, killwords, end)](#apidoc.element.nunjucks.filters.truncate)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>upper (str)](#apidoc.element.nunjucks.filters.upper)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>urlencode (obj)](#apidoc.element.nunjucks.filters.urlencode)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>urlize (str, length, nofollow)](#apidoc.element.nunjucks.filters.urlize)
1.  [function <span class="apidocSignatureSpan">nunjucks.filters.</span>wordcount (str)](#apidoc.element.nunjucks.filters.wordcount)

#### [module nunjucks.lexer](#apidoc.module.nunjucks.lexer)
1.  [function <span class="apidocSignatureSpan">nunjucks.lexer.</span>lex (src, opts)](#apidoc.element.nunjucks.lexer.lex)
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_BLOCK_END
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_BLOCK_START
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_BOOLEAN
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_COLON
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_COMMA
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_COMMENT
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_DATA
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_FLOAT
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_INT
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_LEFT_BRACKET
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_LEFT_CURLY
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_LEFT_PAREN
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_NONE
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_OPERATOR
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_PIPE
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_REGEX
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_RIGHT_BRACKET
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_RIGHT_CURLY
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_RIGHT_PAREN
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_SPECIAL
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_STRING
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_SYMBOL
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_TILDE
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_VARIABLE_END
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_VARIABLE_START
1.  string <span class="apidocSignatureSpan">nunjucks.lexer.</span>TOKEN_WHITESPACE

#### [module nunjucks.lib](#apidoc.module.nunjucks.lib)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>TemplateError (message, lineno, colno)](#apidoc.element.nunjucks.lib.TemplateError)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>asyncFor (obj, iter, cb)](#apidoc.element.nunjucks.lib.asyncFor)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>asyncIter (arr, iter, cb)](#apidoc.element.nunjucks.lib.asyncIter)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>each (obj, func, context)](#apidoc.element.nunjucks.lib.each)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>escape (val)](#apidoc.element.nunjucks.lib.escape)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>extend (obj, obj2)](#apidoc.element.nunjucks.lib.extend)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>groupBy (obj, val)](#apidoc.element.nunjucks.lib.groupBy)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>inOperator (key, val)](#apidoc.element.nunjucks.lib.inOperator)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>indexOf (arr, searchElement, fromIndex)](#apidoc.element.nunjucks.lib.indexOf)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>isArray ()](#apidoc.element.nunjucks.lib.isArray)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>isFunction (obj)](#apidoc.element.nunjucks.lib.isFunction)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>isObject (obj)](#apidoc.element.nunjucks.lib.isObject)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>isString (obj)](#apidoc.element.nunjucks.lib.isString)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>keys (obj)](#apidoc.element.nunjucks.lib.keys)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>map (obj, func)](#apidoc.element.nunjucks.lib.map)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>prettifyError (path, withInternals, err)](#apidoc.element.nunjucks.lib.prettifyError)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>repeat (char_, n)](#apidoc.element.nunjucks.lib.repeat)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>toArray (obj)](#apidoc.element.nunjucks.lib.toArray)
1.  [function <span class="apidocSignatureSpan">nunjucks.lib.</span>without (array)](#apidoc.element.nunjucks.lib.without)

#### [module nunjucks.loaders](#apidoc.module.nunjucks.loaders)
1.  [function <span class="apidocSignatureSpan">nunjucks.loaders.</span>FileSystemLoader ()](#apidoc.element.nunjucks.loaders.FileSystemLoader)
1.  [function <span class="apidocSignatureSpan">nunjucks.loaders.</span>PrecompiledLoader ()](#apidoc.element.nunjucks.loaders.PrecompiledLoader)

#### [module nunjucks.nodes](#apidoc.module.nunjucks.nodes)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Add ()](#apidoc.element.nunjucks.nodes.Add)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>And ()](#apidoc.element.nunjucks.nodes.And)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Array ()](#apidoc.element.nunjucks.nodes.Array)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>AsyncAll ()](#apidoc.element.nunjucks.nodes.AsyncAll)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>AsyncEach ()](#apidoc.element.nunjucks.nodes.AsyncEach)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>BinOp ()](#apidoc.element.nunjucks.nodes.BinOp)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Block ()](#apidoc.element.nunjucks.nodes.Block)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>CallExtension ()](#apidoc.element.nunjucks.nodes.CallExtension)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>CallExtensionAsync ()](#apidoc.element.nunjucks.nodes.CallExtensionAsync)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Caller ()](#apidoc.element.nunjucks.nodes.Caller)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Capture ()](#apidoc.element.nunjucks.nodes.Capture)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Compare ()](#apidoc.element.nunjucks.nodes.Compare)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>CompareOperand ()](#apidoc.element.nunjucks.nodes.CompareOperand)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Concat ()](#apidoc.element.nunjucks.nodes.Concat)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Dict ()](#apidoc.element.nunjucks.nodes.Dict)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Div ()](#apidoc.element.nunjucks.nodes.Div)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Extends ()](#apidoc.element.nunjucks.nodes.Extends)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Filter ()](#apidoc.element.nunjucks.nodes.Filter)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>FilterAsync ()](#apidoc.element.nunjucks.nodes.FilterAsync)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>FloorDiv ()](#apidoc.element.nunjucks.nodes.FloorDiv)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>For ()](#apidoc.element.nunjucks.nodes.For)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>FromImport ()](#apidoc.element.nunjucks.nodes.FromImport)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>FunCall ()](#apidoc.element.nunjucks.nodes.FunCall)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Group ()](#apidoc.element.nunjucks.nodes.Group)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>If ()](#apidoc.element.nunjucks.nodes.If)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>IfAsync ()](#apidoc.element.nunjucks.nodes.IfAsync)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Import ()](#apidoc.element.nunjucks.nodes.Import)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>In ()](#apidoc.element.nunjucks.nodes.In)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Include ()](#apidoc.element.nunjucks.nodes.Include)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>InlineIf ()](#apidoc.element.nunjucks.nodes.InlineIf)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>KeywordArgs ()](#apidoc.element.nunjucks.nodes.KeywordArgs)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Literal ()](#apidoc.element.nunjucks.nodes.Literal)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>LookupVal ()](#apidoc.element.nunjucks.nodes.LookupVal)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Macro ()](#apidoc.element.nunjucks.nodes.Macro)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Mod ()](#apidoc.element.nunjucks.nodes.Mod)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Mul ()](#apidoc.element.nunjucks.nodes.Mul)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Neg ()](#apidoc.element.nunjucks.nodes.Neg)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Node ()](#apidoc.element.nunjucks.nodes.Node)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>NodeList ()](#apidoc.element.nunjucks.nodes.NodeList)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Not ()](#apidoc.element.nunjucks.nodes.Not)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Or ()](#apidoc.element.nunjucks.nodes.Or)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Output ()](#apidoc.element.nunjucks.nodes.Output)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Pair ()](#apidoc.element.nunjucks.nodes.Pair)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Pos ()](#apidoc.element.nunjucks.nodes.Pos)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Pow ()](#apidoc.element.nunjucks.nodes.Pow)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Root ()](#apidoc.element.nunjucks.nodes.Root)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Set ()](#apidoc.element.nunjucks.nodes.Set)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Sub ()](#apidoc.element.nunjucks.nodes.Sub)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Super ()](#apidoc.element.nunjucks.nodes.Super)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Symbol ()](#apidoc.element.nunjucks.nodes.Symbol)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>TemplateData ()](#apidoc.element.nunjucks.nodes.TemplateData)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Value ()](#apidoc.element.nunjucks.nodes.Value)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>printNodes (node, indent)](#apidoc.element.nunjucks.nodes.printNodes)

#### [module nunjucks.nodes.Add](#apidoc.module.nunjucks.nodes.Add)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Add ()](#apidoc.element.nunjucks.nodes.Add.Add)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Add.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Add.extend)

#### [module nunjucks.nodes.Add.prototype](#apidoc.module.nunjucks.nodes.Add.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Add.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Add.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Add.prototype.</span>typename

#### [module nunjucks.nodes.And](#apidoc.module.nunjucks.nodes.And)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>And ()](#apidoc.element.nunjucks.nodes.And.And)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.And.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.And.extend)

#### [module nunjucks.nodes.And.prototype](#apidoc.module.nunjucks.nodes.And.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.And.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.And.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.And.prototype.</span>typename

#### [module nunjucks.nodes.Array](#apidoc.module.nunjucks.nodes.Array)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Array ()](#apidoc.element.nunjucks.nodes.Array.Array)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Array.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Array.extend)

#### [module nunjucks.nodes.Array.prototype](#apidoc.module.nunjucks.nodes.Array.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Array.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Array.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Array.prototype.</span>typename

#### [module nunjucks.nodes.AsyncAll](#apidoc.module.nunjucks.nodes.AsyncAll)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>AsyncAll ()](#apidoc.element.nunjucks.nodes.AsyncAll.AsyncAll)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.AsyncAll.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.AsyncAll.extend)

#### [module nunjucks.nodes.AsyncAll.prototype](#apidoc.module.nunjucks.nodes.AsyncAll.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.AsyncAll.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.AsyncAll.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.AsyncAll.prototype.</span>typename

#### [module nunjucks.nodes.AsyncEach](#apidoc.module.nunjucks.nodes.AsyncEach)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>AsyncEach ()](#apidoc.element.nunjucks.nodes.AsyncEach.AsyncEach)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.AsyncEach.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.AsyncEach.extend)

#### [module nunjucks.nodes.AsyncEach.prototype](#apidoc.module.nunjucks.nodes.AsyncEach.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.AsyncEach.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.AsyncEach.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.AsyncEach.prototype.</span>typename

#### [module nunjucks.nodes.BinOp](#apidoc.module.nunjucks.nodes.BinOp)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>BinOp ()](#apidoc.element.nunjucks.nodes.BinOp.BinOp)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.BinOp.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.BinOp.extend)

#### [module nunjucks.nodes.BinOp.prototype](#apidoc.module.nunjucks.nodes.BinOp.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.BinOp.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.BinOp.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.BinOp.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.BinOp.prototype.</span>typename

#### [module nunjucks.nodes.Block](#apidoc.module.nunjucks.nodes.Block)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Block ()](#apidoc.element.nunjucks.nodes.Block.Block)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Block.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Block.extend)

#### [module nunjucks.nodes.Block.prototype](#apidoc.module.nunjucks.nodes.Block.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Block.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Block.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.Block.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Block.prototype.</span>typename

#### [module nunjucks.nodes.CallExtension](#apidoc.module.nunjucks.nodes.CallExtension)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>CallExtension ()](#apidoc.element.nunjucks.nodes.CallExtension.CallExtension)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.CallExtension.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.CallExtension.extend)

#### [module nunjucks.nodes.CallExtension.prototype](#apidoc.module.nunjucks.nodes.CallExtension.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.CallExtension.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.CallExtension.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.CallExtension.prototype.</span>init (ext, prop, args, contentArgs)](#apidoc.element.nunjucks.nodes.CallExtension.prototype.init)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.CallExtension.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.CallExtension.prototype.</span>typename

#### [module nunjucks.nodes.CallExtensionAsync](#apidoc.module.nunjucks.nodes.CallExtensionAsync)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>CallExtensionAsync ()](#apidoc.element.nunjucks.nodes.CallExtensionAsync.CallExtensionAsync)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.CallExtensionAsync.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.CallExtensionAsync.extend)

#### [module nunjucks.nodes.CallExtensionAsync.prototype](#apidoc.module.nunjucks.nodes.CallExtensionAsync.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.CallExtensionAsync.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.CallExtensionAsync.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.CallExtensionAsync.prototype.</span>typename

#### [module nunjucks.nodes.Caller](#apidoc.module.nunjucks.nodes.Caller)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Caller ()](#apidoc.element.nunjucks.nodes.Caller.Caller)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Caller.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Caller.extend)

#### [module nunjucks.nodes.Caller.prototype](#apidoc.module.nunjucks.nodes.Caller.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Caller.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Caller.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Caller.prototype.</span>typename

#### [module nunjucks.nodes.Capture](#apidoc.module.nunjucks.nodes.Capture)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Capture ()](#apidoc.element.nunjucks.nodes.Capture.Capture)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Capture.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Capture.extend)

#### [module nunjucks.nodes.Capture.prototype](#apidoc.module.nunjucks.nodes.Capture.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Capture.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Capture.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.Capture.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Capture.prototype.</span>typename

#### [module nunjucks.nodes.Compare](#apidoc.module.nunjucks.nodes.Compare)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Compare ()](#apidoc.element.nunjucks.nodes.Compare.Compare)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Compare.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Compare.extend)

#### [module nunjucks.nodes.Compare.prototype](#apidoc.module.nunjucks.nodes.Compare.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Compare.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Compare.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.Compare.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Compare.prototype.</span>typename

#### [module nunjucks.nodes.CompareOperand](#apidoc.module.nunjucks.nodes.CompareOperand)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>CompareOperand ()](#apidoc.element.nunjucks.nodes.CompareOperand.CompareOperand)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.CompareOperand.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.CompareOperand.extend)

#### [module nunjucks.nodes.CompareOperand.prototype](#apidoc.module.nunjucks.nodes.CompareOperand.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.CompareOperand.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.CompareOperand.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.CompareOperand.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.CompareOperand.prototype.</span>typename

#### [module nunjucks.nodes.Concat](#apidoc.module.nunjucks.nodes.Concat)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Concat ()](#apidoc.element.nunjucks.nodes.Concat.Concat)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Concat.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Concat.extend)

#### [module nunjucks.nodes.Concat.prototype](#apidoc.module.nunjucks.nodes.Concat.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Concat.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Concat.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Concat.prototype.</span>typename

#### [module nunjucks.nodes.Dict](#apidoc.module.nunjucks.nodes.Dict)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Dict ()](#apidoc.element.nunjucks.nodes.Dict.Dict)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Dict.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Dict.extend)

#### [module nunjucks.nodes.Dict.prototype](#apidoc.module.nunjucks.nodes.Dict.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Dict.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Dict.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Dict.prototype.</span>typename

#### [module nunjucks.nodes.Div](#apidoc.module.nunjucks.nodes.Div)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Div ()](#apidoc.element.nunjucks.nodes.Div.Div)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Div.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Div.extend)

#### [module nunjucks.nodes.Div.prototype](#apidoc.module.nunjucks.nodes.Div.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Div.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Div.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Div.prototype.</span>typename

#### [module nunjucks.nodes.Extends](#apidoc.module.nunjucks.nodes.Extends)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Extends ()](#apidoc.element.nunjucks.nodes.Extends.Extends)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Extends.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Extends.extend)

#### [module nunjucks.nodes.Extends.prototype](#apidoc.module.nunjucks.nodes.Extends.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Extends.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Extends.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Extends.prototype.</span>typename

#### [module nunjucks.nodes.Filter](#apidoc.module.nunjucks.nodes.Filter)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Filter ()](#apidoc.element.nunjucks.nodes.Filter.Filter)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Filter.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Filter.extend)

#### [module nunjucks.nodes.Filter.prototype](#apidoc.module.nunjucks.nodes.Filter.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Filter.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Filter.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Filter.prototype.</span>typename

#### [module nunjucks.nodes.FilterAsync](#apidoc.module.nunjucks.nodes.FilterAsync)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>FilterAsync ()](#apidoc.element.nunjucks.nodes.FilterAsync.FilterAsync)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.FilterAsync.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.FilterAsync.extend)

#### [module nunjucks.nodes.FilterAsync.prototype](#apidoc.module.nunjucks.nodes.FilterAsync.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.FilterAsync.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.FilterAsync.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.FilterAsync.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.FilterAsync.prototype.</span>typename

#### [module nunjucks.nodes.FloorDiv](#apidoc.module.nunjucks.nodes.FloorDiv)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>FloorDiv ()](#apidoc.element.nunjucks.nodes.FloorDiv.FloorDiv)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.FloorDiv.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.FloorDiv.extend)

#### [module nunjucks.nodes.FloorDiv.prototype](#apidoc.module.nunjucks.nodes.FloorDiv.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.FloorDiv.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.FloorDiv.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.FloorDiv.prototype.</span>typename

#### [module nunjucks.nodes.For](#apidoc.module.nunjucks.nodes.For)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>For ()](#apidoc.element.nunjucks.nodes.For.For)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.For.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.For.extend)

#### [module nunjucks.nodes.For.prototype](#apidoc.module.nunjucks.nodes.For.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.For.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.For.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.For.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.For.prototype.</span>typename

#### [module nunjucks.nodes.FromImport](#apidoc.module.nunjucks.nodes.FromImport)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>FromImport ()](#apidoc.element.nunjucks.nodes.FromImport.FromImport)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.FromImport.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.FromImport.extend)

#### [module nunjucks.nodes.FromImport.prototype](#apidoc.module.nunjucks.nodes.FromImport.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.FromImport.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.FromImport.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.FromImport.prototype.</span>init ()](#apidoc.element.nunjucks.nodes.FromImport.prototype.init)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.FromImport.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.FromImport.prototype.</span>typename

#### [module nunjucks.nodes.FunCall](#apidoc.module.nunjucks.nodes.FunCall)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>FunCall ()](#apidoc.element.nunjucks.nodes.FunCall.FunCall)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.FunCall.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.FunCall.extend)

#### [module nunjucks.nodes.FunCall.prototype](#apidoc.module.nunjucks.nodes.FunCall.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.FunCall.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.FunCall.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.FunCall.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.FunCall.prototype.</span>typename

#### [module nunjucks.nodes.Group](#apidoc.module.nunjucks.nodes.Group)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Group ()](#apidoc.element.nunjucks.nodes.Group.Group)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Group.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Group.extend)

#### [module nunjucks.nodes.Group.prototype](#apidoc.module.nunjucks.nodes.Group.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Group.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Group.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Group.prototype.</span>typename

#### [module nunjucks.nodes.If](#apidoc.module.nunjucks.nodes.If)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>If ()](#apidoc.element.nunjucks.nodes.If.If)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.If.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.If.extend)

#### [module nunjucks.nodes.If.prototype](#apidoc.module.nunjucks.nodes.If.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.If.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.If.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.If.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.If.prototype.</span>typename

#### [module nunjucks.nodes.IfAsync](#apidoc.module.nunjucks.nodes.IfAsync)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>IfAsync ()](#apidoc.element.nunjucks.nodes.IfAsync.IfAsync)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.IfAsync.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.IfAsync.extend)

#### [module nunjucks.nodes.IfAsync.prototype](#apidoc.module.nunjucks.nodes.IfAsync.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.IfAsync.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.IfAsync.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.IfAsync.prototype.</span>typename

#### [module nunjucks.nodes.Import](#apidoc.module.nunjucks.nodes.Import)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Import ()](#apidoc.element.nunjucks.nodes.Import.Import)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Import.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Import.extend)

#### [module nunjucks.nodes.Import.prototype](#apidoc.module.nunjucks.nodes.Import.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Import.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Import.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.Import.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Import.prototype.</span>typename

#### [module nunjucks.nodes.In](#apidoc.module.nunjucks.nodes.In)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>In ()](#apidoc.element.nunjucks.nodes.In.In)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.In.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.In.extend)

#### [module nunjucks.nodes.In.prototype](#apidoc.module.nunjucks.nodes.In.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.In.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.In.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.In.prototype.</span>typename

#### [module nunjucks.nodes.Include](#apidoc.module.nunjucks.nodes.Include)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Include ()](#apidoc.element.nunjucks.nodes.Include.Include)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Include.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Include.extend)

#### [module nunjucks.nodes.Include.prototype](#apidoc.module.nunjucks.nodes.Include.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Include.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Include.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.Include.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Include.prototype.</span>typename

#### [module nunjucks.nodes.InlineIf](#apidoc.module.nunjucks.nodes.InlineIf)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>InlineIf ()](#apidoc.element.nunjucks.nodes.InlineIf.InlineIf)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.InlineIf.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.InlineIf.extend)

#### [module nunjucks.nodes.InlineIf.prototype](#apidoc.module.nunjucks.nodes.InlineIf.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.InlineIf.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.InlineIf.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.InlineIf.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.InlineIf.prototype.</span>typename

#### [module nunjucks.nodes.KeywordArgs](#apidoc.module.nunjucks.nodes.KeywordArgs)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>KeywordArgs ()](#apidoc.element.nunjucks.nodes.KeywordArgs.KeywordArgs)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.KeywordArgs.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.KeywordArgs.extend)

#### [module nunjucks.nodes.KeywordArgs.prototype](#apidoc.module.nunjucks.nodes.KeywordArgs.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.KeywordArgs.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.KeywordArgs.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.KeywordArgs.prototype.</span>typename

#### [module nunjucks.nodes.Literal](#apidoc.module.nunjucks.nodes.Literal)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Literal ()](#apidoc.element.nunjucks.nodes.Literal.Literal)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Literal.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Literal.extend)

#### [module nunjucks.nodes.Literal.prototype](#apidoc.module.nunjucks.nodes.Literal.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Literal.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Literal.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Literal.prototype.</span>typename

#### [module nunjucks.nodes.LookupVal](#apidoc.module.nunjucks.nodes.LookupVal)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>LookupVal ()](#apidoc.element.nunjucks.nodes.LookupVal.LookupVal)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.LookupVal.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.LookupVal.extend)

#### [module nunjucks.nodes.LookupVal.prototype](#apidoc.module.nunjucks.nodes.LookupVal.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.LookupVal.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.LookupVal.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.LookupVal.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.LookupVal.prototype.</span>typename

#### [module nunjucks.nodes.Macro](#apidoc.module.nunjucks.nodes.Macro)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Macro ()](#apidoc.element.nunjucks.nodes.Macro.Macro)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Macro.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Macro.extend)

#### [module nunjucks.nodes.Macro.prototype](#apidoc.module.nunjucks.nodes.Macro.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Macro.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Macro.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.Macro.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Macro.prototype.</span>typename

#### [module nunjucks.nodes.Mod](#apidoc.module.nunjucks.nodes.Mod)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Mod ()](#apidoc.element.nunjucks.nodes.Mod.Mod)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Mod.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Mod.extend)

#### [module nunjucks.nodes.Mod.prototype](#apidoc.module.nunjucks.nodes.Mod.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Mod.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Mod.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Mod.prototype.</span>typename

#### [module nunjucks.nodes.Mul](#apidoc.module.nunjucks.nodes.Mul)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Mul ()](#apidoc.element.nunjucks.nodes.Mul.Mul)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Mul.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Mul.extend)

#### [module nunjucks.nodes.Mul.prototype](#apidoc.module.nunjucks.nodes.Mul.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Mul.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Mul.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Mul.prototype.</span>typename

#### [module nunjucks.nodes.Neg](#apidoc.module.nunjucks.nodes.Neg)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Neg ()](#apidoc.element.nunjucks.nodes.Neg.Neg)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Neg.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Neg.extend)

#### [module nunjucks.nodes.Neg.prototype](#apidoc.module.nunjucks.nodes.Neg.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Neg.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Neg.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Neg.prototype.</span>typename

#### [module nunjucks.nodes.Node](#apidoc.module.nunjucks.nodes.Node)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Node ()](#apidoc.element.nunjucks.nodes.Node.Node)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Node.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Node.extend)

#### [module nunjucks.nodes.Node.prototype](#apidoc.module.nunjucks.nodes.Node.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Node.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Node.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Node.prototype.</span>findAll (type, results)](#apidoc.element.nunjucks.nodes.Node.prototype.findAll)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Node.prototype.</span>init (lineno, colno)](#apidoc.element.nunjucks.nodes.Node.prototype.init)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Node.prototype.</span>iterFields (func)](#apidoc.element.nunjucks.nodes.Node.prototype.iterFields)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Node.prototype.</span>typename

#### [module nunjucks.nodes.NodeList](#apidoc.module.nunjucks.nodes.NodeList)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>NodeList ()](#apidoc.element.nunjucks.nodes.NodeList.NodeList)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.NodeList.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.NodeList.extend)

#### [module nunjucks.nodes.NodeList.prototype](#apidoc.module.nunjucks.nodes.NodeList.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.NodeList.prototype.</span>addChild (node)](#apidoc.element.nunjucks.nodes.NodeList.prototype.addChild)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.NodeList.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.NodeList.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.NodeList.prototype.</span>init ()](#apidoc.element.nunjucks.nodes.NodeList.prototype.init)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.NodeList.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.NodeList.prototype.</span>typename

#### [module nunjucks.nodes.Not](#apidoc.module.nunjucks.nodes.Not)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Not ()](#apidoc.element.nunjucks.nodes.Not.Not)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Not.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Not.extend)

#### [module nunjucks.nodes.Not.prototype](#apidoc.module.nunjucks.nodes.Not.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Not.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Not.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Not.prototype.</span>typename

#### [module nunjucks.nodes.Or](#apidoc.module.nunjucks.nodes.Or)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Or ()](#apidoc.element.nunjucks.nodes.Or.Or)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Or.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Or.extend)

#### [module nunjucks.nodes.Or.prototype](#apidoc.module.nunjucks.nodes.Or.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Or.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Or.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Or.prototype.</span>typename

#### [module nunjucks.nodes.Output](#apidoc.module.nunjucks.nodes.Output)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Output ()](#apidoc.element.nunjucks.nodes.Output.Output)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Output.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Output.extend)

#### [module nunjucks.nodes.Output.prototype](#apidoc.module.nunjucks.nodes.Output.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Output.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Output.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Output.prototype.</span>typename

#### [module nunjucks.nodes.Pair](#apidoc.module.nunjucks.nodes.Pair)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Pair ()](#apidoc.element.nunjucks.nodes.Pair.Pair)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Pair.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Pair.extend)

#### [module nunjucks.nodes.Pair.prototype](#apidoc.module.nunjucks.nodes.Pair.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Pair.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Pair.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.Pair.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Pair.prototype.</span>typename

#### [module nunjucks.nodes.Pos](#apidoc.module.nunjucks.nodes.Pos)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Pos ()](#apidoc.element.nunjucks.nodes.Pos.Pos)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Pos.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Pos.extend)

#### [module nunjucks.nodes.Pos.prototype](#apidoc.module.nunjucks.nodes.Pos.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Pos.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Pos.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Pos.prototype.</span>typename

#### [module nunjucks.nodes.Pow](#apidoc.module.nunjucks.nodes.Pow)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Pow ()](#apidoc.element.nunjucks.nodes.Pow.Pow)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Pow.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Pow.extend)

#### [module nunjucks.nodes.Pow.prototype](#apidoc.module.nunjucks.nodes.Pow.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Pow.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Pow.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Pow.prototype.</span>typename

#### [module nunjucks.nodes.Root](#apidoc.module.nunjucks.nodes.Root)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Root ()](#apidoc.element.nunjucks.nodes.Root.Root)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Root.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Root.extend)

#### [module nunjucks.nodes.Root.prototype](#apidoc.module.nunjucks.nodes.Root.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Root.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Root.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Root.prototype.</span>typename

#### [module nunjucks.nodes.Set](#apidoc.module.nunjucks.nodes.Set)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Set ()](#apidoc.element.nunjucks.nodes.Set.Set)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Set.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Set.extend)

#### [module nunjucks.nodes.Set.prototype](#apidoc.module.nunjucks.nodes.Set.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Set.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Set.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.Set.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Set.prototype.</span>typename

#### [module nunjucks.nodes.Sub](#apidoc.module.nunjucks.nodes.Sub)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Sub ()](#apidoc.element.nunjucks.nodes.Sub.Sub)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Sub.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Sub.extend)

#### [module nunjucks.nodes.Sub.prototype](#apidoc.module.nunjucks.nodes.Sub.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Sub.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Sub.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Sub.prototype.</span>typename

#### [module nunjucks.nodes.Super](#apidoc.module.nunjucks.nodes.Super)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Super ()](#apidoc.element.nunjucks.nodes.Super.Super)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Super.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Super.extend)

#### [module nunjucks.nodes.Super.prototype](#apidoc.module.nunjucks.nodes.Super.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Super.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Super.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.Super.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Super.prototype.</span>typename

#### [module nunjucks.nodes.Symbol](#apidoc.module.nunjucks.nodes.Symbol)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Symbol ()](#apidoc.element.nunjucks.nodes.Symbol.Symbol)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Symbol.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Symbol.extend)

#### [module nunjucks.nodes.Symbol.prototype](#apidoc.module.nunjucks.nodes.Symbol.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Symbol.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Symbol.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Symbol.prototype.</span>typename

#### [module nunjucks.nodes.TemplateData](#apidoc.module.nunjucks.nodes.TemplateData)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>TemplateData ()](#apidoc.element.nunjucks.nodes.TemplateData.TemplateData)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.TemplateData.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.TemplateData.extend)

#### [module nunjucks.nodes.TemplateData.prototype](#apidoc.module.nunjucks.nodes.TemplateData.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.TemplateData.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.TemplateData.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.TemplateData.prototype.</span>typename

#### [module nunjucks.nodes.Value](#apidoc.module.nunjucks.nodes.Value)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Value ()](#apidoc.element.nunjucks.nodes.Value.Value)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Value.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Value.extend)

#### [module nunjucks.nodes.Value.prototype](#apidoc.module.nunjucks.nodes.Value.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.nodes.Value.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Value.prototype.constructor)
1.  object <span class="apidocSignatureSpan">nunjucks.nodes.Value.prototype.</span>fields
1.  string <span class="apidocSignatureSpan">nunjucks.nodes.Value.prototype.</span>typename

#### [module nunjucks.nunjucks](#apidoc.module.nunjucks.nunjucks)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>Environment ()](#apidoc.element.nunjucks.nunjucks.Environment)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>Loader ()](#apidoc.element.nunjucks.nunjucks.Loader)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>PrecompiledLoader ()](#apidoc.element.nunjucks.nunjucks.PrecompiledLoader)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>Template ()](#apidoc.element.nunjucks.nunjucks.Template)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>WebLoader ()](#apidoc.element.nunjucks.nunjucks.WebLoader)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>compile (src, env, path, eagerCompile)](#apidoc.element.nunjucks.nunjucks.compile)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>configure (templatesPath, opts)](#apidoc.element.nunjucks.nunjucks.configure)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>installJinjaCompat ()](#apidoc.element.nunjucks.nunjucks.installJinjaCompat)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>render (name, ctx, cb)](#apidoc.element.nunjucks.nunjucks.render)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>renderString (src, ctx, cb)](#apidoc.element.nunjucks.nunjucks.renderString)
1.  object <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>compiler
1.  object <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>lexer
1.  object <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>lib
1.  object <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>nodes
1.  object <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>parser
1.  object <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>runtime

#### [module nunjucks.nunjucks_slim](#apidoc.module.nunjucks.nunjucks_slim)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>Environment ()](#apidoc.element.nunjucks.nunjucks_slim.Environment)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>Loader ()](#apidoc.element.nunjucks.nunjucks_slim.Loader)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>PrecompiledLoader ()](#apidoc.element.nunjucks.nunjucks_slim.PrecompiledLoader)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>Template ()](#apidoc.element.nunjucks.nunjucks_slim.Template)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>compile (src, env, path, eagerCompile)](#apidoc.element.nunjucks.nunjucks_slim.compile)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>configure (templatesPath, opts)](#apidoc.element.nunjucks.nunjucks_slim.configure)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>installJinjaCompat ()](#apidoc.element.nunjucks.nunjucks_slim.installJinjaCompat)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>render (name, ctx, cb)](#apidoc.element.nunjucks.nunjucks_slim.render)
1.  [function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>renderString (src, ctx, cb)](#apidoc.element.nunjucks.nunjucks_slim.renderString)
1.  object <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>compiler
1.  object <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>lexer
1.  object <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>lib
1.  object <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>nodes
1.  object <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>parser
1.  object <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>runtime

#### [module nunjucks.object](#apidoc.module.nunjucks.object)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>object ()](#apidoc.element.nunjucks.object.object)
1.  [function <span class="apidocSignatureSpan">nunjucks.object.</span>extend (name, props)](#apidoc.element.nunjucks.object.extend)

#### [module nunjucks.object.prototype](#apidoc.module.nunjucks.object.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.object.prototype.</span>constructor ()](#apidoc.element.nunjucks.object.prototype.constructor)
1.  string <span class="apidocSignatureSpan">nunjucks.object.prototype.</span>typename

#### [module nunjucks.parser](#apidoc.module.nunjucks.parser)
1.  [function <span class="apidocSignatureSpan">nunjucks.parser.</span>parse (src, extensions, opts)](#apidoc.element.nunjucks.parser.parse)

#### [module nunjucks.precompile](#apidoc.module.nunjucks.precompile)
1.  [function <span class="apidocSignatureSpan">nunjucks.</span>precompile (input, opts)](#apidoc.element.nunjucks.precompile.precompile)
1.  [function <span class="apidocSignatureSpan">nunjucks.precompile.</span>precompileString (str, opts)](#apidoc.element.nunjucks.precompile.precompileString)

#### [module nunjucks.runtime](#apidoc.module.nunjucks.runtime)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>Frame ()](#apidoc.element.nunjucks.runtime.Frame)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>SafeString (val)](#apidoc.element.nunjucks.runtime.SafeString)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>asyncAll (arr, dimen, func, cb)](#apidoc.element.nunjucks.runtime.asyncAll)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>asyncEach (arr, dimen, iter, cb)](#apidoc.element.nunjucks.runtime.asyncEach)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>callWrap (obj, name, context, args)](#apidoc.element.nunjucks.runtime.callWrap)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>contextOrFrameLookup (context, frame, name)](#apidoc.element.nunjucks.runtime.contextOrFrameLookup)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>copySafeness (dest, target)](#apidoc.element.nunjucks.runtime.copySafeness)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>ensureDefined (val, lineno, colno)](#apidoc.element.nunjucks.runtime.ensureDefined)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>handleError (error, lineno, colno)](#apidoc.element.nunjucks.runtime.handleError)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>inOperator (key, val)](#apidoc.element.nunjucks.runtime.inOperator)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>isArray ()](#apidoc.element.nunjucks.runtime.isArray)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>keys (obj)](#apidoc.element.nunjucks.runtime.keys)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>makeKeywordArgs (obj)](#apidoc.element.nunjucks.runtime.makeKeywordArgs)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>makeMacro (argNames, kwargNames, func)](#apidoc.element.nunjucks.runtime.makeMacro)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>markSafe (val)](#apidoc.element.nunjucks.runtime.markSafe)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>memberLookup (obj, val)](#apidoc.element.nunjucks.runtime.memberLookup)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>numArgs (args)](#apidoc.element.nunjucks.runtime.numArgs)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>suppressValue (val, autoescape)](#apidoc.element.nunjucks.runtime.suppressValue)

#### [module nunjucks.runtime.Frame](#apidoc.module.nunjucks.runtime.Frame)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>Frame ()](#apidoc.element.nunjucks.runtime.Frame.Frame)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.</span>extend (name, props)](#apidoc.element.nunjucks.runtime.Frame.extend)

#### [module nunjucks.runtime.Frame.prototype](#apidoc.module.nunjucks.runtime.Frame.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.prototype.</span>constructor ()](#apidoc.element.nunjucks.runtime.Frame.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.prototype.</span>get (name)](#apidoc.element.nunjucks.runtime.Frame.prototype.get)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.prototype.</span>init (parent, isolateWrites)](#apidoc.element.nunjucks.runtime.Frame.prototype.init)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.prototype.</span>lookup (name)](#apidoc.element.nunjucks.runtime.Frame.prototype.lookup)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.prototype.</span>pop ()](#apidoc.element.nunjucks.runtime.Frame.prototype.pop)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.prototype.</span>push (isolateWrites)](#apidoc.element.nunjucks.runtime.Frame.prototype.push)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.prototype.</span>resolve (name, forWrite)](#apidoc.element.nunjucks.runtime.Frame.prototype.resolve)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.prototype.</span>set (name, val, resolveUp)](#apidoc.element.nunjucks.runtime.Frame.prototype.set)
1.  string <span class="apidocSignatureSpan">nunjucks.runtime.Frame.prototype.</span>typename

#### [module nunjucks.runtime.SafeString](#apidoc.module.nunjucks.runtime.SafeString)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.</span>SafeString (val)](#apidoc.element.nunjucks.runtime.SafeString.SafeString)

#### [module nunjucks.runtime.SafeString.prototype](#apidoc.module.nunjucks.runtime.SafeString.prototype)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.SafeString.prototype.</span>toString ()](#apidoc.element.nunjucks.runtime.SafeString.prototype.toString)
1.  [function <span class="apidocSignatureSpan">nunjucks.runtime.SafeString.prototype.</span>valueOf ()](#apidoc.element.nunjucks.runtime.SafeString.prototype.valueOf)

#### [module nunjucks.transformer](#apidoc.module.nunjucks.transformer)
1.  [function <span class="apidocSignatureSpan">nunjucks.transformer.</span>transform (ast, asyncFilters)](#apidoc.element.nunjucks.transformer.transform)

#### [module nunjucks.web_loaders](#apidoc.module.nunjucks.web_loaders)
1.  [function <span class="apidocSignatureSpan">nunjucks.web_loaders.</span>PrecompiledLoader ()](#apidoc.element.nunjucks.web_loaders.PrecompiledLoader)
1.  [function <span class="apidocSignatureSpan">nunjucks.web_loaders.</span>WebLoader ()](#apidoc.element.nunjucks.web_loaders.WebLoader)



# <a name="apidoc.module.nunjucks"></a>[module nunjucks](#apidoc.module.nunjucks)

#### <a name="apidoc.element.nunjucks.Environment"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>Environment ()](#apidoc.element.nunjucks.Environment)
- description and source-code
```javascript
Environment = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
    else if(loaders.WebLoader) {
        TemplateLoader = new loaders.WebLoader(templatesPath, {
            useCache: opts.web && opts.web.useCache,
            async: opts.web && opts.web.async
        });
    }

    e = new env.Environment(TemplateLoader, opts);

    if(opts && opts.express) {
        e.express(opts.express);
    }

    return e;
};
...
```

#### <a name="apidoc.element.nunjucks.FileSystemLoader"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>FileSystemLoader ()](#apidoc.element.nunjucks.FileSystemLoader)
- description and source-code
```javascript
FileSystemLoader = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
if(lib.isObject(templatesPath)) {
    opts = templatesPath;
    templatesPath = null;
}

var TemplateLoader;
if(loaders.FileSystemLoader) {
    TemplateLoader = new loaders.FileSystemLoader(templatesPath, {
        watch: opts.watch,
        noCache: opts.noCache
    });
}
else if(loaders.WebLoader) {
    TemplateLoader = new loaders.WebLoader(templatesPath, {
        useCache: opts.web && opts.web.useCache,
...
```

#### <a name="apidoc.element.nunjucks.Loader"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>Loader ()](#apidoc.element.nunjucks.Loader)
- description and source-code
```javascript
Loader = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.PrecompiledLoader"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>PrecompiledLoader ()](#apidoc.element.nunjucks.PrecompiledLoader)
- description and source-code
```javascript
PrecompiledLoader = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        }

	        // It's easy to use precompiled templates: just include them
	        // before you configure nunjucks and this will automatically
	        // pick it up and use it
	        if((true) && window.nunjucksPrecompiled) {
	            this.loaders.unshift(
	                new builtin_loaders.PrecompiledLoader(window.nunjucksPrecompiled)
	            );
	        }

	        this.initCache();

	        this.globals = globals();
	        this.filters = {};
...
```

#### <a name="apidoc.element.nunjucks.Template"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>Template ()](#apidoc.element.nunjucks.Template)
- description and source-code
```javascript
Template = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
return e;
};

module.exports.compile = function(src, env, path, eagerCompile) {
if(!e) {
    module.exports.configure();
}
return new module.exports.Template(src, env, path, eagerCompile);
};

module.exports.render = function(name, ctx, cb) {
if(!e) {
    module.exports.configure();
}
...
```

#### <a name="apidoc.element.nunjucks.compile"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>compile (src, env, path, eagerCompile)](#apidoc.element.nunjucks.compile)
- description and source-code
```javascript
compile = function (src, env, path, eagerCompile) {
    if(!e) {
        module.exports.configure();
    }
    return new module.exports.Template(src, env, path, eagerCompile);
}
```
- example usage
```shell
...
	                tmpl = this.loaders[i].cache[_name];
	                if (tmpl) break;
	            }
	        }

	        if(tmpl) {
	            if(eagerCompile) {
	                tmpl.compile();
	            }

	            if(cb) {
	                cb(null, tmpl);
	            }
	            else {
	                return tmpl;
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>compiler.Compiler ()](#apidoc.element.nunjucks.compiler.Compiler)
- description and source-code
```javascript
compiler.Compiler = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.configure"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>configure (templatesPath, opts)](#apidoc.element.nunjucks.configure)
- description and source-code
```javascript
configure = function (templatesPath, opts) {
    opts = opts || {};
    if(lib.isObject(templatesPath)) {
        opts = templatesPath;
        templatesPath = null;
    }

    var TemplateLoader;
    if(loaders.FileSystemLoader) {
        TemplateLoader = new loaders.FileSystemLoader(templatesPath, {
            watch: opts.watch,
            noCache: opts.noCache
        });
    }
    else if(loaders.WebLoader) {
        TemplateLoader = new loaders.WebLoader(templatesPath, {
            useCache: opts.web && opts.web.useCache,
            async: opts.web && opts.web.async
        });
    }

    e = new env.Environment(TemplateLoader, opts);

    if(opts && opts.express) {
        e.express(opts.express);
    }

    return e;
}
```
- example usage
```shell
...
}

return e;
};

module.exports.compile = function(src, env, path, eagerCompile) {
if(!e) {
    module.exports.configure();
}
return new module.exports.Template(src, env, path, eagerCompile);
};

module.exports.render = function(name, ctx, cb) {
if(!e) {
    module.exports.configure();
...
```

#### <a name="apidoc.element.nunjucks.installJinjaCompat"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>installJinjaCompat ()](#apidoc.element.nunjucks.installJinjaCompat)
- description and source-code
```javascript
function installCompat() {
  'use strict';

  // This must be called like 'nunjucks.installCompat' so that 'this'
  // references the nunjucks instance
  var runtime = this.runtime; // jshint ignore:line
  var lib = this.lib; // jshint ignore:line

  var orig_contextOrFrameLookup = runtime.contextOrFrameLookup;
  runtime.contextOrFrameLookup = function(context, frame, key) {
    var val = orig_contextOrFrameLookup.apply(this, arguments);
    if (val === undefined) {
      switch (key) {
      case 'True':
        return true;
      case 'False':
        return false;
      case 'None':
        return null;
      }
    }

    return val;
  };

  var orig_memberLookup = runtime.memberLookup;
  var ARRAY_MEMBERS = {
    pop: function(index) {
      if (index === undefined) {
        return this.pop();
      }
      if (index >= this.length || index < 0) {
        throw new Error('KeyError');
      }
      return this.splice(index, 1);
    },
    append: function(element) {
        return this.push(element);
    },
    remove: function(element) {
      for (var i = 0; i < this.length; i++) {
        if (this[i] === element) {
          return this.splice(i, 1);
        }
      }
      throw new Error('ValueError');
    },
    count: function(element) {
      var count = 0;
      for (var i = 0; i < this.length; i++) {
        if (this[i] === element) {
          count++;
        }
      }
      return count;
    },
    index: function(element) {
      var i;
      if ((i = this.indexOf(element)) === -1) {
        throw new Error('ValueError');
      }
      return i;
    },
    find: function(element) {
      return this.indexOf(element);
    },
    insert: function(index, elem) {
      return this.splice(index, 0, elem);
    }
  };
  var OBJECT_MEMBERS = {
    items: function() {
      var ret = [];
      for(var k in this) {
        ret.push([k, this[k]]);
      }
      return ret;
    },
    values: function() {
      var ret = [];
      for(var k in this) {
        ret.push(this[k]);
      }
      return ret;
    },
    keys: function() {
      var ret = [];
      for(var k in this) {
        ret.push(k);
      }
      return ret;
    },
    get: function(key, def) {
      var output = this[key];
      if (output === undefined) {
        output = def;
      }
      return output;
    },
    has_key: function(key) {
      return this.hasOwnProperty(key);
    },
    pop: function(key, def) {
      var output = this[key];
      if (output === undefined && def !== undefined) {
        output = def;
      } else if (output === undefined) {
        throw new Error('KeyError');
      } else {
        delete this[key];
      }
      return output;
    },
    popitem: function() {
      for (var k in this) {
        // Return the first object pair.
        var val = this[k];
        delete this[k];
        return [k, val];
      }
      throw new Error('KeyError');
    },
    setdefault: function(key, def) {
      if (key in this) {
        return this[key];
      }
      if (def === undefined) {
        def = null;
      }
      return this[key] = def;
    },
    update: function(kwargs) {
      for (var k in kwargs) {
        this[k] = kwargs[k];
      }
      return null;  // Always returns None
    }
  };
  OBJECT_MEMBERS.iteritems = OBJECT_MEMBERS.items;
  OBJECT_MEMBERS.itervalues = OBJECT_MEMBERS.values;
  OBJECT_MEMBERS.iterkeys = OBJECT_MEMBERS.keys;
  runtime.memberLookup = function(obj, val, autoescape) { // jshint ignore:line
    obj = obj || {};

    // If the object is an object, return any of the methods that Python would
    // otherwise provide.
    if (lib.isArray(obj) && ARRAY_MEMBERS.hasOwnProperty(val)) {
      return function() {return ARRAY_MEMBERS[val].apply(obj, arguments);};
    }

    if (lib.isObject(obj) && OBJECT_MEMBERS.hasOwnProperty(val)) {
      return function() {return OBJECT_MEMBERS[val].apply(obj, arguments);};
    }

    return orig_memberLookup.apply(this, arguments);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Add"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Add ()](#apidoc.element.nunjucks.nodes.Add)
- description and source-code
```javascript
nodes.Add = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.And"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.And ()](#apidoc.element.nunjucks.nodes.And)
- description and source-code
```javascript
nodes.And = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Array"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Array ()](#apidoc.element.nunjucks.nodes.Array)
- description and source-code
```javascript
nodes.Array = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.AsyncAll"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.AsyncAll ()](#apidoc.element.nunjucks.nodes.AsyncAll)
- description and source-code
```javascript
nodes.AsyncAll = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.AsyncEach"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.AsyncEach ()](#apidoc.element.nunjucks.nodes.AsyncEach)
- description and source-code
```javascript
nodes.AsyncEach = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.BinOp"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.BinOp ()](#apidoc.element.nunjucks.nodes.BinOp)
- description and source-code
```javascript
nodes.BinOp = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Block"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Block ()](#apidoc.element.nunjucks.nodes.Block)
- description and source-code
```javascript
nodes.Block = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.CallExtension"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.CallExtension ()](#apidoc.element.nunjucks.nodes.CallExtension)
- description and source-code
```javascript
nodes.CallExtension = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.CallExtensionAsync"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.CallExtensionAsync ()](#apidoc.element.nunjucks.nodes.CallExtensionAsync)
- description and source-code
```javascript
nodes.CallExtensionAsync = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Caller"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Caller ()](#apidoc.element.nunjucks.nodes.Caller)
- description and source-code
```javascript
nodes.Caller = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Capture"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Capture ()](#apidoc.element.nunjucks.nodes.Capture)
- description and source-code
```javascript
nodes.Capture = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Compare"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Compare ()](#apidoc.element.nunjucks.nodes.Compare)
- description and source-code
```javascript
nodes.Compare = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.CompareOperand"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.CompareOperand ()](#apidoc.element.nunjucks.nodes.CompareOperand)
- description and source-code
```javascript
nodes.CompareOperand = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Concat"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Concat ()](#apidoc.element.nunjucks.nodes.Concat)
- description and source-code
```javascript
nodes.Concat = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Dict"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Dict ()](#apidoc.element.nunjucks.nodes.Dict)
- description and source-code
```javascript
nodes.Dict = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Div"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Div ()](#apidoc.element.nunjucks.nodes.Div)
- description and source-code
```javascript
nodes.Div = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Extends"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Extends ()](#apidoc.element.nunjucks.nodes.Extends)
- description and source-code
```javascript
nodes.Extends = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Filter"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Filter ()](#apidoc.element.nunjucks.nodes.Filter)
- description and source-code
```javascript
nodes.Filter = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.FilterAsync"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.FilterAsync ()](#apidoc.element.nunjucks.nodes.FilterAsync)
- description and source-code
```javascript
nodes.FilterAsync = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.FloorDiv"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.FloorDiv ()](#apidoc.element.nunjucks.nodes.FloorDiv)
- description and source-code
```javascript
nodes.FloorDiv = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.For"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.For ()](#apidoc.element.nunjucks.nodes.For)
- description and source-code
```javascript
nodes.For = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.FromImport"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.FromImport ()](#apidoc.element.nunjucks.nodes.FromImport)
- description and source-code
```javascript
nodes.FromImport = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.FunCall"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.FunCall ()](#apidoc.element.nunjucks.nodes.FunCall)
- description and source-code
```javascript
nodes.FunCall = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Group"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Group ()](#apidoc.element.nunjucks.nodes.Group)
- description and source-code
```javascript
nodes.Group = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.If"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.If ()](#apidoc.element.nunjucks.nodes.If)
- description and source-code
```javascript
nodes.If = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.IfAsync"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.IfAsync ()](#apidoc.element.nunjucks.nodes.IfAsync)
- description and source-code
```javascript
nodes.IfAsync = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Import"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Import ()](#apidoc.element.nunjucks.nodes.Import)
- description and source-code
```javascript
nodes.Import = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.In"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.In ()](#apidoc.element.nunjucks.nodes.In)
- description and source-code
```javascript
nodes.In = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Include"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Include ()](#apidoc.element.nunjucks.nodes.Include)
- description and source-code
```javascript
nodes.Include = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.InlineIf"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.InlineIf ()](#apidoc.element.nunjucks.nodes.InlineIf)
- description and source-code
```javascript
nodes.InlineIf = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.KeywordArgs"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.KeywordArgs ()](#apidoc.element.nunjucks.nodes.KeywordArgs)
- description and source-code
```javascript
nodes.KeywordArgs = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Literal"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Literal ()](#apidoc.element.nunjucks.nodes.Literal)
- description and source-code
```javascript
nodes.Literal = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.LookupVal"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.LookupVal ()](#apidoc.element.nunjucks.nodes.LookupVal)
- description and source-code
```javascript
nodes.LookupVal = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Macro"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Macro ()](#apidoc.element.nunjucks.nodes.Macro)
- description and source-code
```javascript
nodes.Macro = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Mod"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Mod ()](#apidoc.element.nunjucks.nodes.Mod)
- description and source-code
```javascript
nodes.Mod = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Mul"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Mul ()](#apidoc.element.nunjucks.nodes.Mul)
- description and source-code
```javascript
nodes.Mul = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Neg"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Neg ()](#apidoc.element.nunjucks.nodes.Neg)
- description and source-code
```javascript
nodes.Neg = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Node"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Node ()](#apidoc.element.nunjucks.nodes.Node)
- description and source-code
```javascript
nodes.Node = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.NodeList"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.NodeList ()](#apidoc.element.nunjucks.nodes.NodeList)
- description and source-code
```javascript
nodes.NodeList = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Not"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Not ()](#apidoc.element.nunjucks.nodes.Not)
- description and source-code
```javascript
nodes.Not = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Or"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Or ()](#apidoc.element.nunjucks.nodes.Or)
- description and source-code
```javascript
nodes.Or = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Output"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Output ()](#apidoc.element.nunjucks.nodes.Output)
- description and source-code
```javascript
nodes.Output = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Pair"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Pair ()](#apidoc.element.nunjucks.nodes.Pair)
- description and source-code
```javascript
nodes.Pair = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Pos"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Pos ()](#apidoc.element.nunjucks.nodes.Pos)
- description and source-code
```javascript
nodes.Pos = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Pow"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Pow ()](#apidoc.element.nunjucks.nodes.Pow)
- description and source-code
```javascript
nodes.Pow = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Root"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Root ()](#apidoc.element.nunjucks.nodes.Root)
- description and source-code
```javascript
nodes.Root = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Set"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Set ()](#apidoc.element.nunjucks.nodes.Set)
- description and source-code
```javascript
nodes.Set = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Sub"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Sub ()](#apidoc.element.nunjucks.nodes.Sub)
- description and source-code
```javascript
nodes.Sub = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Super"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Super ()](#apidoc.element.nunjucks.nodes.Super)
- description and source-code
```javascript
nodes.Super = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Symbol"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Symbol ()](#apidoc.element.nunjucks.nodes.Symbol)
- description and source-code
```javascript
nodes.Symbol = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.TemplateData"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.TemplateData ()](#apidoc.element.nunjucks.nodes.TemplateData)
- description and source-code
```javascript
nodes.TemplateData = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Value"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>nodes.Value ()](#apidoc.element.nunjucks.nodes.Value)
- description and source-code
```javascript
nodes.Value = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.object"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>object ()](#apidoc.element.nunjucks.object)
- description and source-code
```javascript
object = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.precompile"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>precompile (input, opts)](#apidoc.element.nunjucks.precompile)
- description and source-code
```javascript
function precompile(input, opts) {
    // The following options are available:
    //
    // * name: name of the template (auto-generated when compiling a directory)
    // * isString: input is a string, not a file path
    // * asFunction: generate a callable function
    // * force: keep compiling on error
    // * env: the Environment to use (gets extensions and async filters from it)
    // * include: which file/folders to include (folders are auto-included, files are auto-excluded)
    // * exclude: which file/folders to exclude (folders are auto-included, files are auto-excluded)
    // * wrapper: function(templates, opts) {...}
    //       Customize the output format to store the compiled template.
    //       By default, templates are stored in a global variable used by the runtime.
    //       A custom loader will be necessary to load your custom wrapper.

    opts = opts || {};
    var env = opts.env || new Environment([]);
    var wrapper = opts.wrapper || precompileGlobal;

    var pathStats = fs.existsSync(input) && fs.statSync(input);
    var precompiled = [];
    var templates = [];

    function addTemplates(dir) {
        var files = fs.readdirSync(dir);

        for(var i=0; i<files.length; i++) {
            var filepath = path.join(dir, files[i]);
            var subpath = filepath.substr(path.join(input, '/').length);
            var stat = fs.statSync(filepath);

            if(stat && stat.isDirectory()) {
                subpath += '/';
                if (!match(subpath, opts.exclude)) {
                    addTemplates(filepath);
                }
            }
            else if(match(subpath, opts.include)) {
                templates.push(filepath);
            }
        }
    }

    if(opts.isString) {
        if(!opts.name) {
            throw new Error('the "name" option is required when ' +
                            'compiling a string');
        }

        precompiled.push( _precompile(
            input,
            opts.name,
            env
        ) );
    }
    else if(pathStats.isFile()) {
        precompiled.push( _precompile(
            fs.readFileSync(input, 'utf-8'),
            opts.name || input,
            env
        ) );
    }
    else if(pathStats.isDirectory()) {
        addTemplates(input);

        for(var i=0; i<templates.length; i++) {
            var name = templates[i].replace(path.join(input, '/'), '');

            try {
                precompiled.push( _precompile(
                    fs.readFileSync(templates[i], 'utf-8'),
                    name,
                    env
                ) );
            } catch(e) {
                if(opts.force) {
                    // Don't stop generating the output if we're
                    // forcing compilation.
                    console.error(e);
                }
                else {
                    throw e;
                }
            }
        }
    }

    return wrapper(precompiled, opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.precompileString"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>precompileString (str, opts)](#apidoc.element.nunjucks.precompileString)
- description and source-code
```javascript
function precompileString(str, opts) {
    opts = opts || {};
    opts.isString = true;
    return precompile(str, opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.render"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>render (name, ctx, cb)](#apidoc.element.nunjucks.render)
- description and source-code
```javascript
render = function (name, ctx, cb) {
    if(!e) {
        module.exports.configure();
    }

    return e.render(name, ctx, cb);
}
```
- example usage
```shell
...
};

module.exports.render = function(name, ctx, cb) {
if(!e) {
    module.exports.configure();
}

return e.render(name, ctx, cb);
};

module.exports.renderString = function(src, ctx, cb) {
if(!e) {
    module.exports.configure();
}
...
```

#### <a name="apidoc.element.nunjucks.renderString"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>renderString (src, ctx, cb)](#apidoc.element.nunjucks.renderString)
- description and source-code
```javascript
renderString = function (src, ctx, cb) {
    if(!e) {
        module.exports.configure();
    }

    return e.renderString(src, ctx, cb);
}
```
- example usage
```shell
...
};

module.exports.renderString = function(src, ctx, cb) {
    if(!e) {
        module.exports.configure();
    }

    return e.renderString(src, ctx, cb);
};

if(precompile) {
    module.exports.precompile = precompile.precompile;
    module.exports.precompileString = precompile.precompileString;
}
...
```

#### <a name="apidoc.element.nunjucks.runtime.Frame"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>runtime.Frame ()](#apidoc.element.nunjucks.runtime.Frame)
- description and source-code
```javascript
runtime.Frame = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.runtime.SafeString"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>runtime.SafeString (val)](#apidoc.element.nunjucks.runtime.SafeString)
- description and source-code
```javascript
function SafeString(val) {
    if(typeof val !== 'string') {
        return val;
    }

    this.val = val;
    this.length = val.length;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.Environment"></a>[module nunjucks.Environment](#apidoc.module.nunjucks.Environment)

#### <a name="apidoc.element.nunjucks.Environment.Environment"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>Environment ()](#apidoc.element.nunjucks.Environment.Environment)
- description and source-code
```javascript
Environment = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
    else if(loaders.WebLoader) {
        TemplateLoader = new loaders.WebLoader(templatesPath, {
            useCache: opts.web && opts.web.useCache,
            async: opts.web && opts.web.async
        });
    }

    e = new env.Environment(TemplateLoader, opts);

    if(opts && opts.express) {
        e.express(opts.express);
    }

    return e;
};
...
```

#### <a name="apidoc.element.nunjucks.Environment.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.</span>extend (name, props)](#apidoc.element.nunjucks.Environment.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.Environment.prototype"></a>[module nunjucks.Environment.prototype](#apidoc.module.nunjucks.Environment.prototype)

#### <a name="apidoc.element.nunjucks.Environment.prototype.addExtension"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>addExtension (name, extension)](#apidoc.element.nunjucks.Environment.prototype.addExtension)
- description and source-code
```javascript
addExtension = function (name, extension) {
    extension._name = name;
    this.extensions[name] = extension;
    this.extensionsList.push(extension);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.Environment.prototype.addFilter"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>addFilter (name, func, async)](#apidoc.element.nunjucks.Environment.prototype.addFilter)
- description and source-code
```javascript
addFilter = function (name, func, async) {
    var wrapped = func;

    if(async) {
        this.asyncFilters.push(name);
    }
    this.filters[name] = wrapped;
    return this;
}
```
- example usage
```shell
...
	        this.globals = globals();
	        this.filters = {};
	        this.asyncFilters = [];
	        this.extensions = {};
	        this.extensionsList = [];

	        for(var name in builtin_filters) {
	            this.addFilter(name, builtin_filters[name]);
	        }
	    },

	    initCache: function() {
	        // Caching and cache busting
	        lib.each(this.loaders, function(loader) {
	            loader.cache = {};
...
```

#### <a name="apidoc.element.nunjucks.Environment.prototype.addGlobal"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>addGlobal (name, value)](#apidoc.element.nunjucks.Environment.prototype.addGlobal)
- description and source-code
```javascript
addGlobal = function (name, value) {
    this.globals[name] = value;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.Environment.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>constructor ()](#apidoc.element.nunjucks.Environment.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.Environment.prototype.express"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>express (app)](#apidoc.element.nunjucks.Environment.prototype.express)
- description and source-code
```javascript
express = function (app) {
    var env = this;

    function NunjucksView(name, opts) {
        this.name          = name;
        this.path          = name;
        this.defaultEngine = opts.defaultEngine;
        this.ext           = path.extname(name);
        if (!this.ext && !this.defaultEngine) throw new Error('No default engine was specified and no extension was provided.');
        if (!this.ext) this.name += (this.ext = ('.' !== this.defaultEngine[0] ? '.' : '') + this.defaultEngine);
    }

    NunjucksView.prototype.render = function(opts, cb) {
      env.render(this.name, opts, cb);
    };

    app.set('view', NunjucksView);
    app.set('nunjucksEnv', this);
    return this;
}
```
- example usage
```shell
...
        async: opts.web && opts.web.async
    });
}

e = new env.Environment(TemplateLoader, opts);

if(opts && opts.express) {
    e.express(opts.express);
}

return e;
};

module.exports.compile = function(src, env, path, eagerCompile) {
if(!e) {
...
```

#### <a name="apidoc.element.nunjucks.Environment.prototype.getExtension"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>getExtension (name)](#apidoc.element.nunjucks.Environment.prototype.getExtension)
- description and source-code
```javascript
getExtension = function (name) {
    return this.extensions[name];
}
```
- example usage
```shell
...
	        extension._name = name;
	        this.extensions[name] = extension;
	        this.extensionsList.push(extension);
	        return this;
	    },

	    removeExtension: function(name) {
	        var extension = this.getExtension(name);
	        if (!extension) return;

	        this.extensionsList = lib.without(this.extensionsList, extension);
	        delete this.extensions[name];
	    },

	    getExtension: function(name) {
...
```

#### <a name="apidoc.element.nunjucks.Environment.prototype.getFilter"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>getFilter (name)](#apidoc.element.nunjucks.Environment.prototype.getFilter)
- description and source-code
```javascript
getFilter = function (name) {
    if(!this.filters[name]) {
        throw new Error('filter not found: ' + name);
    }
    return this.filters[name];
}
```
- example usage
```shell
...

	        this.emit(')');
	    },

	    compileFilter: function(node, frame) {
	        var name = node.name;
	        this.assertType(name, nodes.Symbol);
	        this.emit('env.getFilter("' + name.value + '").call(context, ');
	        this._compileAggregate(node.args, frame);
	        this.emit(')');
	    },

	    compileFilterAsync: function(node, frame) {
	        var name = node.name;
	        this.assertType(name, nodes.Symbol);
...
```

#### <a name="apidoc.element.nunjucks.Environment.prototype.getGlobal"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>getGlobal (name)](#apidoc.element.nunjucks.Environment.prototype.getGlobal)
- description and source-code
```javascript
getGlobal = function (name) {
    if(typeof this.globals[name] === 'undefined') {
        throw new Error('global not found: ' + name);
    }
    return this.globals[name];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.Environment.prototype.getTemplate"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>getTemplate (name, eagerCompile, parentName, ignoreMissing, cb)](#apidoc.element.nunjucks.Environment.prototype.getTemplate)
- description and source-code
```javascript
getTemplate = function (name, eagerCompile, parentName, ignoreMissing, cb) {
    var that = this;
    var tmpl = null;
    if(name && name.raw) {
        // this fixes autoescape for templates referenced in symbols
        name = name.raw;
    }

    if(lib.isFunction(parentName)) {
        cb = parentName;
        parentName = null;
        eagerCompile = eagerCompile || false;
    }

    if(lib.isFunction(eagerCompile)) {
        cb = eagerCompile;
        eagerCompile = false;
    }

    if (name instanceof Template) {
         tmpl = name;
    }
    else if(typeof name !== 'string') {
        throw new Error('template names must be a string: ' + name);
    }
    else {
        for (var i = 0; i < this.loaders.length; i++) {
            var _name = this.resolveTemplate(this.loaders[i], parentName, name);
            tmpl = this.loaders[i].cache[_name];
            if (tmpl) break;
        }
    }

    if(tmpl) {
        if(eagerCompile) {
            tmpl.compile();
        }

        if(cb) {
            cb(null, tmpl);
        }
        else {
            return tmpl;
        }
    } else {
        var syncResult;
        var _this = this;

        var createTemplate = function(err, info) {
            if(!info && !err) {
                if(!ignoreMissing) {
                    err = new Error('template not found: ' + name);
                }
            }

            if (err) {
                if(cb) {
                    cb(err);
                }
                else {
                    throw err;
                }
            }
            else {
                var tmpl;
                if(info) {
                    tmpl = new Template(info.src, _this,
                                        info.path, eagerCompile);

                    if(!info.noCache) {
                        info.loader.cache[name] = tmpl;
                    }
                }
                else {
                    tmpl = new Template('', _this,
                                        '', eagerCompile);
                }

                if(cb) {
                    cb(null, tmpl);
                }
                else {
                    syncResult = tmpl;
                }
            }
        };

        lib.asyncIter(this.loaders, function(loader, i, next, done) {
            function handle(err, src) {
                if(err) {
                    done(err);
                }
                else if(src) {
                    src.loader = loader;
                    done(null, src);
                }
                else {
                    next();
                }
            }

            // Resolve name relative to parentName
            name = that.resolveTemplate(loader, parentName, name);

            if(loader.async) {
                loader.getSource(name, handle);
            }
            else {
                handle(null, loader.getSource(name));
            }
        }, createTemplate);

        return syncResult;
    }
}
```
- example usage
```shell
...

	        // We support a synchronous API to make it easier to migrate
	        // existing code to async. This works because if you don't do
	        // anything async work, the whole thing is actually run
	        // synchronously.
	        var syncResult = null;

	        this.getTemplate(name, function(err, tmpl) {
	            if(err && cb) {
	                callbackAsap(cb, err);
	            }
	            else if(err) {
	                throw err;
	            }
	            else {
...
```

#### <a name="apidoc.element.nunjucks.Environment.prototype.hasExtension"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>hasExtension (name)](#apidoc.element.nunjucks.Environment.prototype.hasExtension)
- description and source-code
```javascript
hasExtension = function (name) {
    return !!this.extensions[name];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.Environment.prototype.init"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>init (loaders, opts)](#apidoc.element.nunjucks.Environment.prototype.init)
- description and source-code
```javascript
init = function (loaders, opts) {
    // The dev flag determines the trace that'll be shown on errors.
    // If set to true, returns the full trace from the error point,
    // otherwise will return trace starting from Template.render
    // (the full trace from within nunjucks may confuse developers using
    //  the library)
    // defaults to false
    opts = this.opts = opts || {};
    this.opts.dev = !!opts.dev;

    // The autoescape flag sets global autoescaping. If true,
    // every string variable will be escaped by default.
    // If false, strings can be manually escaped using the 'escape' filter.
    // defaults to true
    this.opts.autoescape = opts.autoescape != null ? opts.autoescape : true;

    // If true, this will make the system throw errors if trying
    // to output a null or undefined value
    this.opts.throwOnUndefined = !!opts.throwOnUndefined;
    this.opts.trimBlocks = !!opts.trimBlocks;
    this.opts.lstripBlocks = !!opts.lstripBlocks;

    this.loaders = [];

    if(!loaders) {
        // The filesystem loader is only available server-side
        if(builtin_loaders.FileSystemLoader) {
            this.loaders = [new builtin_loaders.FileSystemLoader('views')];
        }
        else if(builtin_loaders.WebLoader) {
            this.loaders = [new builtin_loaders.WebLoader('/views')];
        }
    }
    else {
        this.loaders = lib.isArray(loaders) ? loaders : [loaders];
    }

    // It's easy to use precompiled templates: just include them
    // before you configure nunjucks and this will automatically
    // pick it up and use it
    if(process.env.IS_BROWSER && window.nunjucksPrecompiled) {
        this.loaders.unshift(
            new builtin_loaders.PrecompiledLoader(window.nunjucksPrecompiled)
        );
    }

    this.initCache();

    this.globals = globals();
    this.filters = {};
    this.asyncFilters = [];
    this.extensions = {};
    this.extensionsList = [];

    for(var name in builtin_filters) {
        this.addFilter(name, builtin_filters[name]);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.Environment.prototype.initCache"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>initCache ()](#apidoc.element.nunjucks.Environment.prototype.initCache)
- description and source-code
```javascript
initCache = function () {
    // Caching and cache busting
    lib.each(this.loaders, function(loader) {
        loader.cache = {};

        if(typeof loader.on === 'function') {
            loader.on('update', function(template) {
                loader.cache[template] = null;
            });
        }
    });
}
```
- example usage
```shell
...
	        // pick it up and use it
	        if((true) && window.nunjucksPrecompiled) {
	            this.loaders.unshift(
	                new builtin_loaders.PrecompiledLoader(window.nunjucksPrecompiled)
	            );
	        }

	        this.initCache();

	        this.globals = globals();
	        this.filters = {};
	        this.asyncFilters = [];
	        this.extensions = {};
	        this.extensionsList = [];
...
```

#### <a name="apidoc.element.nunjucks.Environment.prototype.removeExtension"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>removeExtension (name)](#apidoc.element.nunjucks.Environment.prototype.removeExtension)
- description and source-code
```javascript
removeExtension = function (name) {
    var extension = this.getExtension(name);
    if (!extension) return;

    this.extensionsList = lib.without(this.extensionsList, extension);
    delete this.extensions[name];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.Environment.prototype.render"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>render (name, ctx, cb)](#apidoc.element.nunjucks.Environment.prototype.render)
- description and source-code
```javascript
render = function (name, ctx, cb) {
    if(lib.isFunction(ctx)) {
        cb = ctx;
        ctx = null;
    }

    // We support a synchronous API to make it easier to migrate
    // existing code to async. This works because if you don't do
    // anything async work, the whole thing is actually run
    // synchronously.
    var syncResult = null;

    this.getTemplate(name, function(err, tmpl) {
        if(err && cb) {
            callbackAsap(cb, err);
        }
        else if(err) {
            throw err;
        }
        else {
            syncResult = tmpl.render(ctx, cb);
        }
    });

    return syncResult;
}
```
- example usage
```shell
...
};

module.exports.render = function(name, ctx, cb) {
if(!e) {
    module.exports.configure();
}

return e.render(name, ctx, cb);
};

module.exports.renderString = function(src, ctx, cb) {
if(!e) {
    module.exports.configure();
}
...
```

#### <a name="apidoc.element.nunjucks.Environment.prototype.renderString"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>renderString (src, ctx, opts, cb)](#apidoc.element.nunjucks.Environment.prototype.renderString)
- description and source-code
```javascript
renderString = function (src, ctx, opts, cb) {
    if(lib.isFunction(opts)) {
        cb = opts;
        opts = {};
    }
    opts = opts || {};

    var tmpl = new Template(src, this, opts.path);
    return tmpl.render(ctx, cb);
}
```
- example usage
```shell
...
};

module.exports.renderString = function(src, ctx, cb) {
    if(!e) {
        module.exports.configure();
    }

    return e.renderString(src, ctx, cb);
};

if(precompile) {
    module.exports.precompile = precompile.precompile;
    module.exports.precompileString = precompile.precompileString;
}
...
```

#### <a name="apidoc.element.nunjucks.Environment.prototype.resolveTemplate"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>resolveTemplate (loader, parentName, filename)](#apidoc.element.nunjucks.Environment.prototype.resolveTemplate)
- description and source-code
```javascript
resolveTemplate = function (loader, parentName, filename) {
    var isRelative = (loader.isRelative && parentName)? loader.isRelative(filename) : false;
    return (isRelative && loader.resolve)? loader.resolve(parentName, filename) : filename;
}
```
- example usage
```shell
...
	             tmpl = name;
	        }
	        else if(typeof name !== 'string') {
	            throw new Error('template names must be a string: ' + name);
	        }
	        else {
	            for (var i = 0; i < this.loaders.length; i++) {
	                var _name = this.resolveTemplate(this.loaders[i], parentName, name);
	                tmpl = this.loaders[i].cache[_name];
	                if (tmpl) break;
	            }
	        }

	        if(tmpl) {
	            if(eagerCompile) {
...
```

#### <a name="apidoc.element.nunjucks.Environment.prototype.waterfall"></a>[function <span class="apidocSignatureSpan">nunjucks.Environment.prototype.</span>waterfall (tasks, callback, forceAsync)](#apidoc.element.nunjucks.Environment.prototype.waterfall)
- description and source-code
```javascript
waterfall = function (tasks, callback, forceAsync) {
  var nextTick = forceAsync ? executeAsync : executeSync;
  callback = callback || function () {};
  if (!_isArray(tasks)) {
    var err = new Error('First argument to waterfall must be an array of functions');
    return callback(err);
  }
  if (!tasks.length) {
    return callback();
  }
  var wrapIterator = function (iterator) {
    return function (err) {
      if (err) {
        callback.apply(null, arguments);
        callback = function () {};
      } else {
        var args = Array.prototype.slice.call(arguments, 1);
        var next = iterator.next();
        if (next) {
          args.push(wrapIterator(next));
        } else {
          args.push(callback);
        }
        nextTick(function () {
          iterator.apply(null, args);
        });
      }
    };
  };
  wrapIterator(makeIterator(tasks))();
}
```
- example usage
```shell
...
	        this.emitLine('});');

	        this.emitLine('tasks.push(');
	        this.emitLine('function(result, callback){');
	        this.emitLine(this.buffer + ' += result;');
	        this.emitLine('callback(null);');
	        this.emitLine('});');
	        this.emitLine('env.waterfall(tasks, function(){');
	        this.addScopeLevel();
	    },

	    compileTemplateData: function(node, frame) {
	        this.compileLiteral(node, frame);
	    },
...
```



# <a name="apidoc.module.nunjucks.FileSystemLoader"></a>[module nunjucks.FileSystemLoader](#apidoc.module.nunjucks.FileSystemLoader)

#### <a name="apidoc.element.nunjucks.FileSystemLoader.FileSystemLoader"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>FileSystemLoader ()](#apidoc.element.nunjucks.FileSystemLoader.FileSystemLoader)
- description and source-code
```javascript
FileSystemLoader = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
if(lib.isObject(templatesPath)) {
    opts = templatesPath;
    templatesPath = null;
}

var TemplateLoader;
if(loaders.FileSystemLoader) {
    TemplateLoader = new loaders.FileSystemLoader(templatesPath, {
        watch: opts.watch,
        noCache: opts.noCache
    });
}
else if(loaders.WebLoader) {
    TemplateLoader = new loaders.WebLoader(templatesPath, {
        useCache: opts.web && opts.web.useCache,
...
```

#### <a name="apidoc.element.nunjucks.FileSystemLoader.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.FileSystemLoader.</span>extend (name, props)](#apidoc.element.nunjucks.FileSystemLoader.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.FileSystemLoader.prototype"></a>[module nunjucks.FileSystemLoader.prototype](#apidoc.module.nunjucks.FileSystemLoader.prototype)

#### <a name="apidoc.element.nunjucks.FileSystemLoader.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.FileSystemLoader.prototype.</span>constructor ()](#apidoc.element.nunjucks.FileSystemLoader.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.FileSystemLoader.prototype.getSource"></a>[function <span class="apidocSignatureSpan">nunjucks.FileSystemLoader.prototype.</span>getSource (name)](#apidoc.element.nunjucks.FileSystemLoader.prototype.getSource)
- description and source-code
```javascript
getSource = function (name) {
    var fullpath = null;
    var paths = this.searchPaths;

    for(var i=0; i<paths.length; i++) {
        var basePath = path.resolve(paths[i]);
        var p = path.resolve(paths[i], name);

        // Only allow the current directory and anything
        // underneath it to be searched
        if(p.indexOf(basePath) === 0 && existsSync(p)) {
            fullpath = p;
            break;
        }
    }

    if(!fullpath) {
        return null;
    }

    this.pathsToNames[fullpath] = name;

    return { src: fs.readFileSync(fullpath, 'utf-8'),
             path: fullpath,
             noCache: this.noCache };
}
```
- example usage
```shell
...
	                    }
	                }

	                // Resolve name relative to parentName
	                name = that.resolveTemplate(loader, parentName, name);

	                if(loader.async) {
	                    loader.getSource(name, handle);
	                }
	                else {
	                    handle(null, loader.getSource(name));
	                }
	            }, createTemplate);

	            return syncResult;
...
```

#### <a name="apidoc.element.nunjucks.FileSystemLoader.prototype.init"></a>[function <span class="apidocSignatureSpan">nunjucks.FileSystemLoader.prototype.</span>init (searchPaths, opts)](#apidoc.element.nunjucks.FileSystemLoader.prototype.init)
- description and source-code
```javascript
init = function (searchPaths, opts) {
    if(typeof opts === 'boolean') {
        console.log(
            '[nunjucks] Warning: you passed a boolean as the second ' +
            'argument to FileSystemLoader, but it now takes an options ' +
            'object. See http://mozilla.github.io/nunjucks/api.html#filesystemloader'
        );
    }

    opts = opts || {};
    this.pathsToNames = {};
    this.noCache = !!opts.noCache;

    if(searchPaths) {
        searchPaths = lib.isArray(searchPaths) ? searchPaths : [searchPaths];
        // For windows, convert to forward slashes
        this.searchPaths = searchPaths.map(path.normalize);
    }
    else {
        this.searchPaths = ['.'];
    }

    if(opts.watch) {
        // Watch all the templates in the paths and fire an event when
        // they change
        var chokidar = require('chokidar');
        var paths = this.searchPaths.filter(function(p) { return existsSync(p); });
        var watcher = chokidar.watch(paths);
        var _this = this;
        watcher.on('all', function(event, fullname) {
            fullname = path.resolve(fullname);
            if(event === 'change' && fullname in _this.pathsToNames) {
                _this.emit('update', _this.pathsToNames[fullname]);
            }
        });
        watcher.on('error', function(error) {
            console.log('Watcher error: ' + error);
        });
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.Loader"></a>[module nunjucks.Loader](#apidoc.module.nunjucks.Loader)

#### <a name="apidoc.element.nunjucks.Loader.Loader"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>Loader ()](#apidoc.element.nunjucks.Loader.Loader)
- description and source-code
```javascript
Loader = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.Loader.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.Loader.</span>extend (name, props)](#apidoc.element.nunjucks.Loader.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.Loader.prototype"></a>[module nunjucks.Loader.prototype](#apidoc.module.nunjucks.Loader.prototype)

#### <a name="apidoc.element.nunjucks.Loader.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.Loader.prototype.</span>constructor ()](#apidoc.element.nunjucks.Loader.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.Loader.prototype.emit"></a>[function <span class="apidocSignatureSpan">nunjucks.Loader.prototype.</span>emit (name)](#apidoc.element.nunjucks.Loader.prototype.emit)
- description and source-code
```javascript
emit = function (name) {
    var args = Array.prototype.slice.call(arguments, 1);

    if(this.listeners && this.listeners[name]) {
        lib.each(this.listeners[name], function(listener) {
            listener.apply(null, args);
        });
    }
}
```
- example usage
```shell
...
	    '>=': '>='
	};

	// A common pattern is to emit binary operators
	function binOpEmitter(str) {
	    return function(node, frame) {
	        this.compile(node.left, frame);
	        this.emit(str);
	        this.compile(node.right, frame);
	    };
	}

	var Compiler = Object.extend({
	    init: function(templateName, throwOnUndefined) {
	        this.templateName = templateName;
...
```

#### <a name="apidoc.element.nunjucks.Loader.prototype.isRelative"></a>[function <span class="apidocSignatureSpan">nunjucks.Loader.prototype.</span>isRelative (filename)](#apidoc.element.nunjucks.Loader.prototype.isRelative)
- description and source-code
```javascript
isRelative = function (filename) {
    return (filename.indexOf('./') === 0 || filename.indexOf('../') === 0);
}
```
- example usage
```shell
...
	        if(!this.filters[name]) {
	            throw new Error('filter not found: ' + name);
	        }
	        return this.filters[name];
	    },

	    resolveTemplate: function(loader, parentName, filename) {
	        var isRelative = (loader.isRelative && parentName)? loader.isRelative(filename) : false;
	        return (isRelative && loader.resolve)? loader.resolve(parentName, filename) : filename;
	    },

	    getTemplate: function(name, eagerCompile, parentName, ignoreMissing, cb) {
	        var that = this;
	        var tmpl = null;
	        if(name && name.raw) {
...
```

#### <a name="apidoc.element.nunjucks.Loader.prototype.on"></a>[function <span class="apidocSignatureSpan">nunjucks.Loader.prototype.</span>on (name, func)](#apidoc.element.nunjucks.Loader.prototype.on)
- description and source-code
```javascript
on = function (name, func) {
    this.listeners = this.listeners || {};
    this.listeners[name] = this.listeners[name] || [];
    this.listeners[name].push(func);
}
```
- example usage
```shell
...

	    initCache: function() {
	        // Caching and cache busting
	        lib.each(this.loaders, function(loader) {
	            loader.cache = {};

	            if(typeof loader.on === 'function') {
	                loader.on('update', function(template) {
	                    loader.cache[template] = null;
	                });
	            }
	        });
	    },

	    addExtension: function(name, extension) {
...
```

#### <a name="apidoc.element.nunjucks.Loader.prototype.resolve"></a>[function <span class="apidocSignatureSpan">nunjucks.Loader.prototype.</span>resolve (from, to)](#apidoc.element.nunjucks.Loader.prototype.resolve)
- description and source-code
```javascript
resolve = function (from, to) {
    return path.resolve(path.dirname(from), to);
}
```
- example usage
```shell
...
	            throw new Error('filter not found: ' + name);
	        }
	        return this.filters[name];
	    },

	    resolveTemplate: function(loader, parentName, filename) {
	        var isRelative = (loader.isRelative && parentName)? loader.isRelative(filename) : false;
	        return (isRelative && loader.resolve)? loader.resolve(parentName, filename) : filename;
	    },

	    getTemplate: function(name, eagerCompile, parentName, ignoreMissing, cb) {
	        var that = this;
	        var tmpl = null;
	        if(name && name.raw) {
	            // this fixes autoescape for templates referenced in symbols
...
```



# <a name="apidoc.module.nunjucks.PrecompiledLoader"></a>[module nunjucks.PrecompiledLoader](#apidoc.module.nunjucks.PrecompiledLoader)

#### <a name="apidoc.element.nunjucks.PrecompiledLoader.PrecompiledLoader"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>PrecompiledLoader ()](#apidoc.element.nunjucks.PrecompiledLoader.PrecompiledLoader)
- description and source-code
```javascript
PrecompiledLoader = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        }

	        // It's easy to use precompiled templates: just include them
	        // before you configure nunjucks and this will automatically
	        // pick it up and use it
	        if((true) && window.nunjucksPrecompiled) {
	            this.loaders.unshift(
	                new builtin_loaders.PrecompiledLoader(window.nunjucksPrecompiled)
	            );
	        }

	        this.initCache();

	        this.globals = globals();
	        this.filters = {};
...
```

#### <a name="apidoc.element.nunjucks.PrecompiledLoader.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.PrecompiledLoader.</span>extend (name, props)](#apidoc.element.nunjucks.PrecompiledLoader.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.PrecompiledLoader.prototype"></a>[module nunjucks.PrecompiledLoader.prototype](#apidoc.module.nunjucks.PrecompiledLoader.prototype)

#### <a name="apidoc.element.nunjucks.PrecompiledLoader.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.PrecompiledLoader.prototype.</span>constructor ()](#apidoc.element.nunjucks.PrecompiledLoader.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.PrecompiledLoader.prototype.getSource"></a>[function <span class="apidocSignatureSpan">nunjucks.PrecompiledLoader.prototype.</span>getSource (name)](#apidoc.element.nunjucks.PrecompiledLoader.prototype.getSource)
- description and source-code
```javascript
getSource = function (name) {
    if (this.precompiled[name]) {
        return {
            src: { type: 'code',
                   obj: this.precompiled[name] },
            path: name
        };
    }
    return null;
}
```
- example usage
```shell
...
	                    }
	                }

	                // Resolve name relative to parentName
	                name = that.resolveTemplate(loader, parentName, name);

	                if(loader.async) {
	                    loader.getSource(name, handle);
	                }
	                else {
	                    handle(null, loader.getSource(name));
	                }
	            }, createTemplate);

	            return syncResult;
...
```

#### <a name="apidoc.element.nunjucks.PrecompiledLoader.prototype.init"></a>[function <span class="apidocSignatureSpan">nunjucks.PrecompiledLoader.prototype.</span>init (compiledTemplates)](#apidoc.element.nunjucks.PrecompiledLoader.prototype.init)
- description and source-code
```javascript
init = function (compiledTemplates) {
    this.precompiled = compiledTemplates || {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.Template"></a>[module nunjucks.Template](#apidoc.module.nunjucks.Template)

#### <a name="apidoc.element.nunjucks.Template.Template"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>Template ()](#apidoc.element.nunjucks.Template.Template)
- description and source-code
```javascript
Template = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
return e;
};

module.exports.compile = function(src, env, path, eagerCompile) {
if(!e) {
    module.exports.configure();
}
return new module.exports.Template(src, env, path, eagerCompile);
};

module.exports.render = function(name, ctx, cb) {
if(!e) {
    module.exports.configure();
}
...
```

#### <a name="apidoc.element.nunjucks.Template.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.Template.</span>extend (name, props)](#apidoc.element.nunjucks.Template.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.Template.prototype"></a>[module nunjucks.Template.prototype](#apidoc.module.nunjucks.Template.prototype)

#### <a name="apidoc.element.nunjucks.Template.prototype._compile"></a>[function <span class="apidocSignatureSpan">nunjucks.Template.prototype.</span>_compile ()](#apidoc.element.nunjucks.Template.prototype._compile)
- description and source-code
```javascript
_compile = function () {
    var props;

    if(this.tmplProps) {
        props = this.tmplProps;
    }
    else {
        var source = compiler.compile(this.tmplStr,
                                      this.env.asyncFilters,
                                      this.env.extensionsList,
                                      this.path,
                                      this.env.opts);

<span class="apidocCodeCommentSpan">        /* jslint evil: true */
</span>        var func = new Function(source);
        props = func();
    }

    this.blocks = this._getBlocks(props);
    this.rootRenderFunc = props.root;
    this.compiled = true;
}
```
- example usage
```shell
...
	        }

	        this.path = path;

	        if(eagerCompile) {
	            var _this = this;
	            try {
	                _this._compile();
	            }
	            catch(err) {
	                throw lib.prettifyError(this.path, this.env.opts.dev, err);
	            }
	        }
	        else {
	            this.compiled = false;
...
```

#### <a name="apidoc.element.nunjucks.Template.prototype._getBlocks"></a>[function <span class="apidocSignatureSpan">nunjucks.Template.prototype.</span>_getBlocks (props)](#apidoc.element.nunjucks.Template.prototype._getBlocks)
- description and source-code
```javascript
_getBlocks = function (props) {
    var blocks = {};

    for(var k in props) {
        if(k.slice(0, 2) === 'b_') {
            blocks[k.slice(2)] = props[k];
        }
    }

    return blocks;
}
```
- example usage
```shell
...
	                                          this.env.opts);

	            /* jslint evil: true */
	            var func = new Function(source);
	            props = func();
	        }

	        this.blocks = this._getBlocks(props);
	        this.rootRenderFunc = props.root;
	        this.compiled = true;
	    },

	    _getBlocks: function(props) {
	        var blocks = {};
...
```

#### <a name="apidoc.element.nunjucks.Template.prototype.compile"></a>[function <span class="apidocSignatureSpan">nunjucks.Template.prototype.</span>compile ()](#apidoc.element.nunjucks.Template.prototype.compile)
- description and source-code
```javascript
compile = function () {
    if(!this.compiled) {
        this._compile();
    }
}
```
- example usage
```shell
...
	                tmpl = this.loaders[i].cache[_name];
	                if (tmpl) break;
	            }
	        }

	        if(tmpl) {
	            if(eagerCompile) {
	                tmpl.compile();
	            }

	            if(cb) {
	                cb(null, tmpl);
	            }
	            else {
	                return tmpl;
...
```

#### <a name="apidoc.element.nunjucks.Template.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.Template.prototype.</span>constructor ()](#apidoc.element.nunjucks.Template.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.Template.prototype.getExported"></a>[function <span class="apidocSignatureSpan">nunjucks.Template.prototype.</span>getExported (ctx, parentFrame, cb)](#apidoc.element.nunjucks.Template.prototype.getExported)
- description and source-code
```javascript
getExported = function (ctx, parentFrame, cb) {
    if (typeof ctx === 'function') {
        cb = ctx;
        ctx = {};
    }

    if (typeof parentFrame === 'function') {
        cb = parentFrame;
        parentFrame = null;
    }

    // Catch compile errors for async rendering
    try {
        this.compile();
    } catch (e) {
        if (cb) return cb(e);
        else throw e;
    }

    var frame = parentFrame ? parentFrame.push() : new Frame();
    frame.topLevel = true;

    // Run the rootRenderFunc to populate the context with exported vars
    var context = new Context(ctx || {}, this.blocks, this.env);
    this.rootRenderFunc(this.env,
                        context,
                        frame,
                        runtime,
                        function(err) {
    		        if ( err ) {
    			    cb(err, null);
    		        } else {
    			    cb(null, context.getExported());
    		        }
                        });
}
```
- example usage
```shell
...
	                            context,
	                            frame,
	                            runtime,
	                            function(err) {
	        		        if ( err ) {
	        			    cb(err, null);
	        		        } else {
	        			    cb(null, context.getExported());
	        		        }
	                            });
	    },

	    compile: function() {
	        if(!this.compiled) {
	            this._compile();
...
```

#### <a name="apidoc.element.nunjucks.Template.prototype.init"></a>[function <span class="apidocSignatureSpan">nunjucks.Template.prototype.</span>init (src, env, path, eagerCompile)](#apidoc.element.nunjucks.Template.prototype.init)
- description and source-code
```javascript
init = function (src, env, path, eagerCompile) {
    this.env = env || new Environment();

    if(lib.isObject(src)) {
        switch(src.type) {
        case 'code': this.tmplProps = src.obj; break;
        case 'string': this.tmplStr = src.obj; break;
        }
    }
    else if(lib.isString(src)) {
        this.tmplStr = src;
    }
    else {
        throw new Error('src must be a string or an object describing ' +
                        'the source');
    }

    this.path = path;

    if(eagerCompile) {
        var _this = this;
        try {
            _this._compile();
        }
        catch(err) {
            throw lib.prettifyError(this.path, this.env.opts.dev, err);
        }
    }
    else {
        this.compiled = false;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.Template.prototype.render"></a>[function <span class="apidocSignatureSpan">nunjucks.Template.prototype.</span>render (ctx, parentFrame, cb)](#apidoc.element.nunjucks.Template.prototype.render)
- description and source-code
```javascript
render = function (ctx, parentFrame, cb) {
    if (typeof ctx === 'function') {
        cb = ctx;
        ctx = {};
    }
    else if (typeof parentFrame === 'function') {
        cb = parentFrame;
        parentFrame = null;
    }

    var forceAsync = true;
    if(parentFrame) {
        // If there is a frame, we are being called from internal
        // code of another template, and the internal system
        // depends on the sync/async nature of the parent template
        // to be inherited, so force an async callback
        forceAsync = false;
    }

    var _this = this;
    // Catch compile errors for async rendering
    try {
        _this.compile();
    } catch (_err) {
        var err = lib.prettifyError(this.path, this.env.opts.dev, _err);
        if (cb) return callbackAsap(cb, err);
        else throw err;
    }

    var context = new Context(ctx || {}, _this.blocks, _this.env);
    var frame = parentFrame ? parentFrame.push(true) : new Frame();
    frame.topLevel = true;
    var syncResult = null;

    _this.rootRenderFunc(
        _this.env,
        context,
        frame || new Frame(),
        runtime,
        function(err, res) {
            if(err) {
                err = lib.prettifyError(_this.path, _this.env.opts.dev, err);
            }

            if(cb) {
                if(forceAsync) {
                    callbackAsap(cb, err, res);
                }
                else {
                    cb(err, res);
                }
            }
            else {
                if(err) { throw err; }
                syncResult = res;
            }
        }
    );

    return syncResult;
}
```
- example usage
```shell
...
};

module.exports.render = function(name, ctx, cb) {
if(!e) {
    module.exports.configure();
}

return e.render(name, ctx, cb);
};

module.exports.renderString = function(src, ctx, cb) {
if(!e) {
    module.exports.configure();
}
...
```



# <a name="apidoc.module.nunjucks.compiler"></a>[module nunjucks.compiler](#apidoc.module.nunjucks.compiler)

#### <a name="apidoc.element.nunjucks.compiler.Compiler"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.</span>Compiler ()](#apidoc.element.nunjucks.compiler.Compiler)
- description and source-code
```javascript
Compiler = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.compile"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.</span>compile (src, asyncFilters, extensions, name, opts)](#apidoc.element.nunjucks.compiler.compile)
- description and source-code
```javascript
compile = function (src, asyncFilters, extensions, name, opts) {
    var c = new Compiler(name, opts.throwOnUndefined);

    // Run the extension preprocessors against the source.
    if(extensions && extensions.length) {
        for(var i=0; i<extensions.length; i++) {
            if('preprocess' in extensions[i]) {
                src = extensions[i].preprocess(src, name);
            }
        }
    }

    c.compile(transformer.transform(
        parser.parse(src,
                     extensions,
                     opts),
        asyncFilters,
        name
    ));
    return c.getCode();
}
```
- example usage
```shell
...
	                tmpl = this.loaders[i].cache[_name];
	                if (tmpl) break;
	            }
	        }

	        if(tmpl) {
	            if(eagerCompile) {
	                tmpl.compile();
	            }

	            if(cb) {
	                cb(null, tmpl);
	            }
	            else {
	                return tmpl;
...
```



# <a name="apidoc.module.nunjucks.compiler.Compiler"></a>[module nunjucks.compiler.Compiler](#apidoc.module.nunjucks.compiler.Compiler)

#### <a name="apidoc.element.nunjucks.compiler.Compiler.Compiler"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.</span>Compiler ()](#apidoc.element.nunjucks.compiler.Compiler.Compiler)
- description and source-code
```javascript
Compiler = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.</span>extend (name, props)](#apidoc.element.nunjucks.compiler.Compiler.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.compiler.Compiler.prototype"></a>[module nunjucks.compiler.Compiler.prototype](#apidoc.module.nunjucks.compiler.Compiler.prototype)

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype._compileAggregate"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>_compileAggregate (node, frame, startChar, endChar)](#apidoc.element.nunjucks.compiler.Compiler.prototype._compileAggregate)
- description and source-code
```javascript
_compileAggregate = function (node, frame, startChar, endChar) {
    if(startChar) {
        this.emit(startChar);
    }

    for(var i=0; i<node.children.length; i++) {
        if(i > 0) {
            this.emit(',');
        }

        this.compile(node.children[i], frame);
    }

    if(endChar) {
        this.emit(endChar);
    }
}
```
- example usage
```shell
...
	        else {
	            this.emit('runtime.contextOrFrameLookup(' +
	                      'context, frame, "' + name + '")');
	        }
	    },

	    compileGroup: function(node, frame) {
	        this._compileAggregate(node, frame, '(', ')');
	    },

	    compileArray: function(node, frame) {
	        this._compileAggregate(node, frame, '[', ']');
	    },

	    compileDict: function(node, frame) {
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype._compileAsyncLoop"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>_compileAsyncLoop (node, frame, parallel)](#apidoc.element.nunjucks.compiler.Compiler.prototype._compileAsyncLoop)
- description and source-code
```javascript
_compileAsyncLoop = function (node, frame, parallel) {
    // This shares some code with the For tag, but not enough to
    // worry about. This iterates across an object asynchronously,
    // but not in parallel.

    var i = this.tmpid();
    var len = this.tmpid();
    var arr = this.tmpid();
    var asyncMethod = parallel ? 'asyncAll' : 'asyncEach';
    frame = frame.push();

    this.emitLine('frame = frame.push();');

    this.emit('var ' + arr + ' = ');
    this._compileExpression(node.arr, frame);
    this.emitLine(';');

    if(node.name instanceof nodes.Array) {
        this.emit('runtime.' + asyncMethod + '(' + arr + ', ' +
                  node.name.children.length + ', function(');

        lib.each(node.name.children, function(name) {
            this.emit(name.value + ',');
        }, this);

        this.emit(i + ',' + len + ',next) {');

        lib.each(node.name.children, function(name) {
            var id = name.value;
            frame.set(id, id);
            this.emitLine('frame.set("' + id + '", ' + id + ');');
        }, this);
    }
    else {
        var id = node.name.value;
        this.emitLine('runtime.' + asyncMethod + '(' + arr + ', 1, function(' + id + ', ' + i + ', ' + len + ',next) {');
        this.emitLine('frame.set("' + id + '", ' + id + ');');
        frame.set(id, id);
    }

    this.emitLoopBindings(node, arr, i, len);

    this.withScopedSyntax(function() {
        var buf;
        if(parallel) {
            buf = this.tmpid();
            this.pushBufferId(buf);
        }

        this.compile(node.body, frame);
        this.emitLine('next(' + i + (buf ? ',' + buf : '') + ');');

        if(parallel) {
            this.popBufferId();
        }
    });

    var output = this.tmpid();
    this.emitLine('}, ' + this.makeCallback(output));
    this.addScopeLevel();

    if(parallel) {
        this.emitLine(this.buffer + ' += ' + output + ';');
    }

    if (node.else_) {
      this.emitLine('if (!' + arr + '.length) {');
      this.compile(node.else_, frame);
      this.emitLine('}');
    }

    this.emitLine('frame = frame.pop();');
}
```
- example usage
```shell
...
	          this.emitLine('}');
	        }

	        this.emitLine('frame = frame.pop();');
	    },

	    compileAsyncEach: function(node, frame) {
	        this._compileAsyncLoop(node, frame);
	    },

	    compileAsyncAll: function(node, frame) {
	        this._compileAsyncLoop(node, frame, true);
	    },

	    _compileMacro: function(node) {
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype._compileChildren"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>_compileChildren (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype._compileChildren)
- description and source-code
```javascript
_compileChildren = function (node, frame) {
    var children = node.children;
    for(var i=0, l=children.length; i<l; i++) {
        this.compile(children[i], frame);
    }
}
```
- example usage
```shell
...
	    },

	    compileCallExtensionAsync: function(node, frame) {
	        this.compileCallExtension(node, frame, true);
	    },

	    compileNodeList: function(node, frame) {
	        this._compileChildren(node, frame);
	    },

	    compileLiteral: function(node) {
	        if(typeof node.value === 'string') {
	            var val = node.value.replace(/\\/g, '\\\\');
	            val = val.replace(/"/g, '\\"');
	            val = val.replace(/\n/g, '\\n');
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype._compileExpression"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>_compileExpression (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype._compileExpression)
- description and source-code
```javascript
_compileExpression = function (node, frame) {
    // TODO: I'm not really sure if this type check is worth it or
    // not.
    this.assertType(
        node,
        nodes.Literal,
        nodes.Symbol,
        nodes.Group,
        nodes.Array,
        nodes.Dict,
        nodes.FunCall,
        nodes.Caller,
        nodes.Filter,
        nodes.LookupVal,
        nodes.Compare,
        nodes.InlineIf,
        nodes.In,
        nodes.And,
        nodes.Or,
        nodes.Not,
        nodes.Add,
        nodes.Concat,
        nodes.Sub,
        nodes.Mul,
        nodes.Div,
        nodes.FloorDiv,
        nodes.Mod,
        nodes.Pow,
        nodes.Neg,
        nodes.Pos,
        nodes.Compare,
        nodes.NodeList
    );
    this.compile(node, frame);
}
```
- example usage
```shell
...
	                          'use 'parser.parseSignature'');
	            }

	            lib.each(args.children, function(arg, i) {
	                // Tag arguments are passed normally to the call. Note
	                // that keyword arguments are turned into a single js
	                // object as the last argument, if they exist.
	                this._compileExpression(arg, frame);

	                if(i !== args.children.length - 1 || contentArgs.length) {
	                    this.emit(',');
	                }
	            }, this);
	        }
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype._compileMacro"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>_compileMacro (node)](#apidoc.element.nunjucks.compiler.Compiler.prototype._compileMacro)
- description and source-code
```javascript
_compileMacro = function (node) {
    var args = [];
    var kwargs = null;
    var funcId = 'macro_' + this.tmpid();

    // Type check the definition of the args
    lib.each(node.args.children, function(arg, i) {
        if(i === node.args.children.length - 1 &&
           arg instanceof nodes.Dict) {
            kwargs = arg;
        }
        else {
            this.assertType(arg, nodes.Symbol);
            args.push(arg);
        }
    }, this);

    var realNames = lib.map(args, function(n) { return 'l_' + n.value; });
    realNames.push('kwargs');

    // Quoted argument names
    var argNames = lib.map(args, function(n) { return '"' + n.value + '"'; });
    var kwargNames = lib.map((kwargs && kwargs.children) || [],
                             function(n) { return '"' + n.key.value + '"'; });

    // We pass a function to makeMacro which destructures the
    // arguments so support setting positional args with keywords
    // args and passing keyword args as positional args
    // (essentially default values). See runtime.js.
    var frame = new Frame();
    this.emitLines(
        'var ' + funcId + ' = runtime.makeMacro(',
        '[' + argNames.join(', ') + '], ',
        '[' + kwargNames.join(', ') + '], ',
        'function (' + realNames.join(', ') + ') {',
        'var callerFrame = frame;',
        'frame = new runtime.Frame();',
        'kwargs = kwargs || {};',
        'if (kwargs.hasOwnProperty("caller")) {',
        'frame.set("caller", kwargs.caller); }'
    );

    // Expose the arguments to the template. Don't need to use
    // random names because the function
    // will create a new run-time scope for us
    lib.each(args, function(arg) {
        this.emitLine('frame.set("' + arg.value + '", ' +
                      'l_' + arg.value + ');');
        frame.set(arg.value, 'l_' + arg.value);
    }, this);

    // Expose the keyword arguments
    if(kwargs) {
        lib.each(kwargs.children, function(pair) {
            var name = pair.key.value;
            this.emit('frame.set("' + name + '", ' +
                      'kwargs.hasOwnProperty("' + name + '") ? ' +
                      'kwargs["' + name + '"] : ');
            this._compileExpression(pair.value, frame);
            this.emitLine(');');
        }, this);
    }

    var bufferId = this.tmpid();
    this.pushBufferId(bufferId);

    this.withScopedSyntax(function () {
      this.compile(node.body, frame);
    });

    this.emitLine('frame = callerFrame;');
    this.emitLine('return new runtime.SafeString(' + bufferId + ');');
    this.emitLine('});');
    this.popBufferId();

    return funcId;
}
```
- example usage
```shell
...
	        this.emitLine('});');
	        this.popBufferId();

	        return funcId;
	    },

	    compileMacro: function(node, frame) {
	        var funcId = this._compileMacro(node, frame);

	        // Expose the macro to the templates
	        var name = node.name.value;
	        frame.set(name, funcId);

	        if(frame.parent) {
	            this.emitLine('frame.set("' + name + '", ' + funcId + ');');
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype._getNodeName"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>_getNodeName (node)](#apidoc.element.nunjucks.compiler.Compiler.prototype._getNodeName)
- description and source-code
```javascript
_getNodeName = function (node) {
    switch (node.typename) {
        case 'Symbol':
            return node.value;
        case 'FunCall':
            return 'the return value of (' + this._getNodeName(node.name) + ')';
        case 'LookupVal':
            return this._getNodeName(node.target) + '["' +
                   this._getNodeName(node.val) + '"]';
        case 'Literal':
            return node.value.toString();
        default:
            return '--expression--';
    }
}
```
- example usage
```shell
...
	    },

	    _getNodeName: function(node) {
	        switch (node.typename) {
	            case 'Symbol':
	                return node.value;
	            case 'FunCall':
	                return 'the return value of (' + this._getNodeName(node.name) + ')';
	            case 'LookupVal':
	                return this._getNodeName(node.target) + '["' +
	                       this._getNodeName(node.val) + '"]';
	            case 'Literal':
	                return node.value.toString();
	            default:
	                return '--expression--';
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype._templateName"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>_templateName ()](#apidoc.element.nunjucks.compiler.Compiler.prototype._templateName)
- description and source-code
```javascript
_templateName = function () {
    return this.templateName == null? 'undefined' : JSON.stringify(this.templateName);
}
```
- example usage
```shell
...

	    compileImport: function(node, frame) {
	        var id = this.tmpid();
	        var target = node.target.value;

	        this.emit('env.getTemplate(');
	        this._compileExpression(node.template, frame);
	        this.emitLine(', false, '+this._templateName()+', false, ' + this.makeCallback(id));
	        this.addScopeLevel();

	        this.emitLine(id + '.getExported(' +
	            (node.withContext ? 'context.getVariables(), frame, ' : '') +
	            this.makeCallback(id));
	        this.addScopeLevel();
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.addScopeLevel"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>addScopeLevel ()](#apidoc.element.nunjucks.compiler.Compiler.prototype.addScopeLevel)
- description and source-code
```javascript
addScopeLevel = function () {
    this.scopeClosers += '})';
}
```
- example usage
```shell
...
	            }, this);
	        }

	        if(async) {
	            var res = this.tmpid();
	            this.emitLine(', ' + this.makeCallback(res));
	            this.emitLine(this.buffer + ' += runtime.suppressValue(' + res + ', ' + autoescape + ' && env.opts.autoescape);');
	            this.addScopeLevel();
	        }
	        else {
	            this.emit(')');
	            this.emit(', ' + autoescape + ' && env.opts.autoescape);\n');
	        }
	    },
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.assertType"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>assertType (node)](#apidoc.element.nunjucks.compiler.Compiler.prototype.assertType)
- description and source-code
```javascript
assertType = function (node) {
    var types = lib.toArray(arguments).slice(1);
    var success = false;

    for(var i=0; i<types.length; i++) {
        if(node instanceof types[i]) {
            success = true;
        }
    }

    if(!success) {
        this.fail('assertType: invalid type: ' + node.typename,
                  node.lineno,
                  node.colno);
    }
}
```
- example usage
```shell
...
	            this.emit(endChar);
	        }
	    },

	    _compileExpression: function(node, frame) {
	        // TODO: I'm not really sure if this type check is worth it or
	        // not.
	        this.assertType(
	            node,
	            nodes.Literal,
	            nodes.Symbol,
	            nodes.Group,
	            nodes.Array,
	            nodes.Dict,
	            nodes.FunCall,
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.closeScopeLevels"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>closeScopeLevels ()](#apidoc.element.nunjucks.compiler.Compiler.prototype.closeScopeLevels)
- description and source-code
```javascript
closeScopeLevels = function () {
    this.emitLine(this.scopeClosers + ';');
    this.scopeClosers = '';
}
```
- example usage
```shell
...
	    },

	    emitFuncEnd: function(noReturn) {
	        if(!noReturn) {
	            this.emitLine('cb(null, ' + this.buffer +');');
	        }

	        this.closeScopeLevels();
	        this.emitLine('} catch (e) {');
	        this.emitLine('  cb(runtime.handleError(e, lineno, colno));');
	        this.emitLine('}');
	        this.emitLine('}');
	        this.buffer = null;
	    },
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compile"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compile (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compile)
- description and source-code
```javascript
compile = function (node, frame) {
    var _compile = this['compile' + node.typename];
    if(_compile) {
        _compile.call(this, node, frame);
    }
    else {
        this.fail('compile: Cannot compile node: ' + node.typename,
                  node.lineno,
                  node.colno);
    }
}
```
- example usage
```shell
...
	                tmpl = this.loaders[i].cache[_name];
	                if (tmpl) break;
	            }
	        }

	        if(tmpl) {
	            if(eagerCompile) {
	                tmpl.compile();
	            }

	            if(cb) {
	                cb(null, tmpl);
	            }
	            else {
	                return tmpl;
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileAdd"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileAdd (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileAdd)
- description and source-code
```javascript
compileAdd = function (node, frame) {
    this.compile(node.left, frame);
    this.emit(str);
    this.compile(node.right, frame);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileAnd"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileAnd (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileAnd)
- description and source-code
```javascript
compileAnd = function (node, frame) {
    this.compile(node.left, frame);
    this.emit(str);
    this.compile(node.right, frame);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileArray"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileArray (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileArray)
- description and source-code
```javascript
compileArray = function (node, frame) {
    this._compileAggregate(node, frame, '[', ']');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileAsyncAll"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileAsyncAll (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileAsyncAll)
- description and source-code
```javascript
compileAsyncAll = function (node, frame) {
    this._compileAsyncLoop(node, frame, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileAsyncEach"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileAsyncEach (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileAsyncEach)
- description and source-code
```javascript
compileAsyncEach = function (node, frame) {
    this._compileAsyncLoop(node, frame);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileBlock"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileBlock (node)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileBlock)
- description and source-code
```javascript
compileBlock = function (node) {
    var id = this.tmpid();

    // If we are executing outside a block (creating a top-level
    // block), we really don't want to execute its code because it
    // will execute twice: once when the child template runs and
    // again when the parent template runs. Note that blocks
    // within blocks will *always* execute immediately *and*
    // wherever else they are invoked (like used in a parent
    // template). This may have behavioral differences from jinja
    // because blocks can have side effects, but it seems like a
    // waste of performance to always execute huge top-level
    // blocks twice
    if(!this.inBlock) {
        this.emit('(parentTemplate ? function(e, c, f, r, cb) { cb(""); } : ');
    }
    this.emit('context.getBlock("' + node.name.value + '")');
    if(!this.inBlock) {
        this.emit(')');
    }
    this.emitLine('(env, context, frame, runtime, ' + this.makeCallback(id));
    this.emitLine(this.buffer + ' += ' + id + ';');
    this.addScopeLevel();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileCallExtension"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileCallExtension (node, frame, async)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileCallExtension)
- description and source-code
```javascript
compileCallExtension = function (node, frame, async) {
    var args = node.args;
    var contentArgs = node.contentArgs;
    var autoescape = typeof node.autoescape === 'boolean' ? node.autoescape : true;

    if(!async) {
        this.emit(this.buffer + ' += runtime.suppressValue(');
    }

    this.emit('env.getExtension("' + node.extName + '")["' + node.prop + '"](');
    this.emit('context');

    if(args || contentArgs) {
        this.emit(',');
    }

    if(args) {
        if(!(args instanceof nodes.NodeList)) {
            this.fail('compileCallExtension: arguments must be a NodeList, ' +
                      'use 'parser.parseSignature'');
        }

        lib.each(args.children, function(arg, i) {
            // Tag arguments are passed normally to the call. Note
            // that keyword arguments are turned into a single js
            // object as the last argument, if they exist.
            this._compileExpression(arg, frame);

            if(i !== args.children.length - 1 || contentArgs.length) {
                this.emit(',');
            }
        }, this);
    }

    if(contentArgs.length) {
        lib.each(contentArgs, function(arg, i) {
            if(i > 0) {
                this.emit(',');
            }

            if(arg) {
                var id = this.tmpid();

                this.emitLine('function(cb) {');
                this.emitLine('if(!cb) { cb = function(err) { if(err) { throw err; }}}');
                this.pushBufferId(id);

                this.withScopedSyntax(function() {
                    this.compile(arg, frame);
                    this.emitLine('cb(null, ' + id + ');');
                });

                this.popBufferId();
                this.emitLine('return ' + id + ';');
                this.emitLine('}');
            }
            else {
                this.emit('null');
            }
        }, this);
    }

    if(async) {
        var res = this.tmpid();
        this.emitLine(', ' + this.makeCallback(res));
        this.emitLine(this.buffer + ' += runtime.suppressValue(' + res + ', ' + autoescape + ' && env.opts.autoescape);');
        this.addScopeLevel();
    }
    else {
        this.emit(')');
        this.emit(', ' + autoescape + ' && env.opts.autoescape);\n');
    }
}
```
- example usage
```shell
...
	        else {
	            this.emit(')');
	            this.emit(', ' + autoescape + ' && env.opts.autoescape);\n');
	        }
	    },

	    compileCallExtensionAsync: function(node, frame) {
	        this.compileCallExtension(node, frame, true);
	    },

	    compileNodeList: function(node, frame) {
	        this._compileChildren(node, frame);
	    },

	    compileLiteral: function(node) {
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileCallExtensionAsync"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileCallExtensionAsync (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileCallExtensionAsync)
- description and source-code
```javascript
compileCallExtensionAsync = function (node, frame) {
    this.compileCallExtension(node, frame, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileCaller"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileCaller (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileCaller)
- description and source-code
```javascript
compileCaller = function (node, frame) {
    // basically an anonymous "macro expression"
    this.emit('(function (){');
    var funcId = this._compileMacro(node, frame);
    this.emit('return ' + funcId + ';})()');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileCapture"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileCapture (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileCapture)
- description and source-code
```javascript
compileCapture = function (node, frame) {
    this.emitLine('(function() {');
    this.emitLine('var output = "";');
    this.withScopedSyntax(function () {
        this.compile(node.body, frame);
    });
    this.emitLine('return output;');
    this.emitLine('})()');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileCompare"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileCompare (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileCompare)
- description and source-code
```javascript
compileCompare = function (node, frame) {
    this.compile(node.expr, frame);

    for(var i=0; i<node.ops.length; i++) {
        var n = node.ops[i];
        this.emit(' ' + compareOps[n.type] + ' ');
        this.compile(n.expr, frame);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileConcat"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileConcat (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileConcat)
- description and source-code
```javascript
compileConcat = function (node, frame) {
    this.compile(node.left, frame);
    this.emit(str);
    this.compile(node.right, frame);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileDict"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileDict (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileDict)
- description and source-code
```javascript
compileDict = function (node, frame) {
    this._compileAggregate(node, frame, '{', '}');
}
```
- example usage
```shell
...
	        var names = [];

	        lib.each(node.children, function(pair) {
	            names.push(pair.key.value);
	        });

	        this.emit('runtime.makeKeywordArgs(');
	        this.compileDict(node, frame);
	        this.emit(')');
	    },

	    compileSet: function(node, frame) {
	        var ids = [];

	        // Lookup the variable names for each identifier and create
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileDiv"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileDiv (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileDiv)
- description and source-code
```javascript
compileDiv = function (node, frame) {
    this.compile(node.left, frame);
    this.emit(str);
    this.compile(node.right, frame);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileExtends"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileExtends (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileExtends)
- description and source-code
```javascript
compileExtends = function (node, frame) {
    var k = this.tmpid();

    this.emit('env.getTemplate(');
    this._compileExpression(node.template, frame);
    this.emitLine(', true, '+this._templateName()+', false, ' + this.makeCallback('_parentTemplate'));

    // extends is a dynamic tag and can occur within a block like
    // 'if', so if this happens we need to capture the parent
    // template in the top-level scope
    this.emitLine('parentTemplate = _parentTemplate');

    this.emitLine('for(var ' + k + ' in parentTemplate.blocks) {');
    this.emitLine('context.addBlock(' + k +
                  ', parentTemplate.blocks[' + k + ']);');
    this.emitLine('}');

    this.addScopeLevel();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileFilter"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileFilter (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileFilter)
- description and source-code
```javascript
compileFilter = function (node, frame) {
    var name = node.name;
    this.assertType(name, nodes.Symbol);
    this.emit('env.getFilter("' + name.value + '").call(context, ');
    this._compileAggregate(node.args, frame);
    this.emit(')');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileFilterAsync"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileFilterAsync (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileFilterAsync)
- description and source-code
```javascript
compileFilterAsync = function (node, frame) {
    var name = node.name;
    this.assertType(name, nodes.Symbol);

    var symbol = node.symbol.value;
    frame.set(symbol, symbol);

    this.emit('env.getFilter("' + name.value + '").call(context, ');
    this._compileAggregate(node.args, frame);
    this.emitLine(', ' + this.makeCallback(symbol));

    this.addScopeLevel();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileFloorDiv"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileFloorDiv (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileFloorDiv)
- description and source-code
```javascript
compileFloorDiv = function (node, frame) {
    this.emit('Math.floor(');
    this.compile(node.left, frame);
    this.emit(' / ');
    this.compile(node.right, frame);
    this.emit(')');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileFor"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileFor (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileFor)
- description and source-code
```javascript
compileFor = function (node, frame) {
    // Some of this code is ugly, but it keeps the generated code
    // as fast as possible. ForAsync also shares some of this, but
    // not much.

    var v;
    var i = this.tmpid();
    var len = this.tmpid();
    var arr = this.tmpid();
    frame = frame.push();

    this.emitLine('frame = frame.push();');

    this.emit('var ' + arr + ' = ');
    this._compileExpression(node.arr, frame);
    this.emitLine(';');

    this.emit('if(' + arr + ') {');

    // If multiple names are passed, we need to bind them
    // appropriately
    if(node.name instanceof nodes.Array) {
        this.emitLine('var ' + i + ';');

        // The object could be an arroy or object. Note that the
        // body of the loop is duplicated for each condition, but
        // we are optimizing for speed over size.
        this.emitLine('if(runtime.isArray(' + arr + ')) {'); {
            this.emitLine('var ' + len + ' = ' + arr + '.length;');
            this.emitLine('for(' + i + '=0; ' + i + ' < ' + arr + '.length; '
                          + i + '++) {');

            // Bind each declared var
            for (var u=0; u < node.name.children.length; u++) {
                var tid = this.tmpid();
                this.emitLine('var ' + tid + ' = ' + arr + '[' + i + '][' + u + ']');
                this.emitLine('frame.set("' + node.name.children[u].value
                              + '", ' + arr + '[' + i + '][' + u + ']' + ');');
                frame.set(node.name.children[u].value, tid);
            }

            this.emitLoopBindings(node, arr, i, len);
            this.withScopedSyntax(function() {
                this.compile(node.body, frame);
            });
            this.emitLine('}');
        }

        this.emitLine('} else {'); {
            // Iterate over the key/values of an object
            var key = node.name.children[0];
            var val = node.name.children[1];
            var k = this.tmpid();
            v = this.tmpid();
            frame.set(key.value, k);
            frame.set(val.value, v);

            this.emitLine(i + ' = -1;');
            this.emitLine('var ' + len + ' = runtime.keys(' + arr + ').length;');
            this.emitLine('for(var ' + k + ' in ' + arr + ') {');
            this.emitLine(i + '++;');
            this.emitLine('var ' + v + ' = ' + arr + '[' + k + '];');
            this.emitLine('frame.set("' + key.value + '", ' + k + ');');
            this.emitLine('frame.set("' + val.value + '", ' + v + ');');

            this.emitLoopBindings(node, arr, i, len);
            this.withScopedSyntax(function() {
                this.compile(node.body, frame);
            });
            this.emitLine('}');
        }

        this.emitLine('}');
    }
    else {
        // Generate a typical array iteration
        v = this.tmpid();
        frame.set(node.name.value, v);

        this.emitLine('var ' + len + ' = ' + arr + '.length;');
        this.emitLine('for(var ' + i + '=0; ' + i + ' < ' + arr + '.length; ' +
                      i + '++) {');
        this.emitLine('var ' + v + ' = ' + arr + '[' + i + '];');
        this.emitLine('frame.set("' + node.name.value + '", ' + v + ');');

        this.emitLoopBindings(node, arr, i, len);

        this.withScopedSyntax(function() {
            this.compile(node.body, frame);
        });

        this.emitLine('}');
    }

    this.emitLine('}');
    if (node.else_) {
      this.emitLine('if (!' + len + ') {');
      this.compile(node.else_, frame);
      this.emitLine('}');
    }

    this.emitLine('frame = frame.pop();');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileFromImport"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileFromImport (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileFromImport)
- description and source-code
```javascript
compileFromImport = function (node, frame) {
    var importedId = this.tmpid();

    this.emit('env.getTemplate(');
    this._compileExpression(node.template, frame);
    this.emitLine(', false, '+this._templateName()+', false, ' + this.makeCallback(importedId));
    this.addScopeLevel();

    this.emitLine(importedId + '.getExported(' +
        (node.withContext ? 'context.getVariables(), frame, ' : '') +
        this.makeCallback(importedId));
    this.addScopeLevel();

    lib.each(node.names.children, function(nameNode) {
        var name;
        var alias;
        var id = this.tmpid();

        if(nameNode instanceof nodes.Pair) {
            name = nameNode.key.value;
            alias = nameNode.value.value;
        }
        else {
            name = nameNode.value;
            alias = name;
        }

        this.emitLine('if(' + importedId + '.hasOwnProperty("' + name + '")) {');
        this.emitLine('var ' + id + ' = ' + importedId + '.' + name + ';');
        this.emitLine('} else {');
        this.emitLine('cb(new Error("cannot import \'' + name + '\'")); return;');
        this.emitLine('}');

        frame.set(alias, id);

        if(frame.parent) {
            this.emitLine('frame.set("' + alias + '", ' + id + ');');
        }
        else {
            this.emitLine('context.setVariable("' + alias + '", ' + id + ');');
        }
    }, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileFunCall"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileFunCall (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileFunCall)
- description and source-code
```javascript
compileFunCall = function (node, frame) {
    // Keep track of line/col info at runtime by settings
    // variables within an expression. An expression in javascript
    // like (x, y, z) returns the last value, and x and y can be
    // anything
    this.emit('(lineno = ' + node.lineno +
              ', colno = ' + node.colno + ', ');

    this.emit('runtime.callWrap(');
    // Compile it as normal.
    this._compileExpression(node.name, frame);

    // Output the name of what we're calling so we can get friendly errors
    // if the lookup fails.
    this.emit(', "' + this._getNodeName(node.name).replace(/"/g, '\\"') + '", context, ');

    this._compileAggregate(node.args, frame, '[', '])');

    this.emit(')');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileGroup"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileGroup (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileGroup)
- description and source-code
```javascript
compileGroup = function (node, frame) {
    this._compileAggregate(node, frame, '(', ')');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileIf"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileIf (node, frame, async)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileIf)
- description and source-code
```javascript
compileIf = function (node, frame, async) {
    this.emit('if(');
    this._compileExpression(node.cond, frame);
    this.emitLine(') {');

    this.withScopedSyntax(function() {
        this.compile(node.body, frame);

        if(async) {
            this.emit('cb()');
        }
    });

    if(node.else_) {
        this.emitLine('}\nelse {');

        this.withScopedSyntax(function() {
            this.compile(node.else_, frame);

            if(async) {
                this.emit('cb()');
            }
        });
    } else if(async) {
        this.emitLine('}\nelse {');
        this.emit('cb()');
    }

    this.emitLine('}');
}
```
- example usage
```shell
...
	        }

	        this.emitLine('}');
	    },

	    compileIfAsync: function(node, frame) {
	        this.emit('(function(cb) {');
	        this.compileIf(node, frame, true);
	        this.emit('})(' + this.makeCallback());
	        this.addScopeLevel();
	    },

	    emitLoopBindings: function(node, arr, i, len) {
	        var bindings = {
	            index: i + ' + 1',
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileIfAsync"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileIfAsync (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileIfAsync)
- description and source-code
```javascript
compileIfAsync = function (node, frame) {
    this.emit('(function(cb) {');
    this.compileIf(node, frame, true);
    this.emit('})(' + this.makeCallback());
    this.addScopeLevel();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileImport"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileImport (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileImport)
- description and source-code
```javascript
compileImport = function (node, frame) {
    var id = this.tmpid();
    var target = node.target.value;

    this.emit('env.getTemplate(');
    this._compileExpression(node.template, frame);
    this.emitLine(', false, '+this._templateName()+', false, ' + this.makeCallback(id));
    this.addScopeLevel();

    this.emitLine(id + '.getExported(' +
        (node.withContext ? 'context.getVariables(), frame, ' : '') +
        this.makeCallback(id));
    this.addScopeLevel();

    frame.set(target, id);

    if(frame.parent) {
        this.emitLine('frame.set("' + target + '", ' + id + ');');
    }
    else {
        this.emitLine('context.setVariable("' + target + '", ' + id + ');');
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileIn"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileIn (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileIn)
- description and source-code
```javascript
compileIn = function (node, frame) {
  this.emit('runtime.inOperator(');
  this.compile(node.left, frame);
  this.emit(',');
  this.compile(node.right, frame);
  this.emit(')');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileInclude"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileInclude (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileInclude)
- description and source-code
```javascript
compileInclude = function (node, frame) {
    var id = this.tmpid();
    var id2 = this.tmpid();

    this.emitLine('var tasks = [];');
    this.emitLine('tasks.push(');
    this.emitLine('function(callback) {');
    this.emit('env.getTemplate(');
    this._compileExpression(node.template, frame);
    this.emitLine(', false, '+this._templateName()+', ' + node.ignoreMissing + ', ' + this.makeCallback(id));
    this.emitLine('callback(null,' + id + ');});');
    this.emitLine('});');

    this.emitLine('tasks.push(');
    this.emitLine('function(template, callback){');
    this.emitLine('template.render(' +
        'context.getVariables(), frame, ' + this.makeCallback(id2));
    this.emitLine('callback(null,' + id2 + ');});');
    this.emitLine('});');

    this.emitLine('tasks.push(');
    this.emitLine('function(result, callback){');
    this.emitLine(this.buffer + ' += result;');
    this.emitLine('callback(null);');
    this.emitLine('});');
    this.emitLine('env.waterfall(tasks, function(){');
    this.addScopeLevel();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileInlineIf"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileInlineIf (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileInlineIf)
- description and source-code
```javascript
compileInlineIf = function (node, frame) {
    this.emit('(');
    this.compile(node.cond, frame);
    this.emit('?');
    this.compile(node.body, frame);
    this.emit(':');
    if(node.else_ !== null)
        this.compile(node.else_, frame);
    else
        this.emit('""');
    this.emit(')');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileKeywordArgs"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileKeywordArgs (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileKeywordArgs)
- description and source-code
```javascript
compileKeywordArgs = function (node, frame) {
    var names = [];

    lib.each(node.children, function(pair) {
        names.push(pair.key.value);
    });

    this.emit('runtime.makeKeywordArgs(');
    this.compileDict(node, frame);
    this.emit(')');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileLiteral"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileLiteral (node)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileLiteral)
- description and source-code
```javascript
compileLiteral = function (node) {
    if(typeof node.value === 'string') {
        var val = node.value.replace(/\\/g, '\\\\');
        val = val.replace(/"/g, '\\"');
        val = val.replace(/\n/g, '\\n');
        val = val.replace(/\r/g, '\\r');
        val = val.replace(/\t/g, '\\t');
        this.emit('"' + val  + '"');
    }
    else if (node.value === null) {
        this.emit('null');
    }
    else {
        this.emit(node.value.toString());
    }
}
```
- example usage
```shell
...
	        this.emitLine('callback(null);');
	        this.emitLine('});');
	        this.emitLine('env.waterfall(tasks, function(){');
	        this.addScopeLevel();
	    },

	    compileTemplateData: function(node, frame) {
	        this.compileLiteral(node, frame);
	    },

	    compileCapture: function(node, frame) {
	        this.emitLine('(function() {');
	        this.emitLine('var output = "";');
	        this.withScopedSyntax(function () {
	            this.compile(node.body, frame);
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileLookupVal"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileLookupVal (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileLookupVal)
- description and source-code
```javascript
compileLookupVal = function (node, frame) {
    this.emit('runtime.memberLookup((');
    this._compileExpression(node.target, frame);
    this.emit('),');
    this._compileExpression(node.val, frame);
    this.emit(')');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileMacro"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileMacro (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileMacro)
- description and source-code
```javascript
compileMacro = function (node, frame) {
    var funcId = this._compileMacro(node, frame);

    // Expose the macro to the templates
    var name = node.name.value;
    frame.set(name, funcId);

    if(frame.parent) {
        this.emitLine('frame.set("' + name + '", ' + funcId + ');');
    }
    else {
        if(node.name.value.charAt(0) !== '_') {
            this.emitLine('context.addExport("' + name + '");');
        }
        this.emitLine('context.setVariable("' + name + '", ' + funcId + ');');
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileMod"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileMod (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileMod)
- description and source-code
```javascript
compileMod = function (node, frame) {
    this.compile(node.left, frame);
    this.emit(str);
    this.compile(node.right, frame);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileMul"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileMul (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileMul)
- description and source-code
```javascript
compileMul = function (node, frame) {
    this.compile(node.left, frame);
    this.emit(str);
    this.compile(node.right, frame);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileNeg"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileNeg (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileNeg)
- description and source-code
```javascript
compileNeg = function (node, frame) {
    this.emit('-');
    this.compile(node.target, frame);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileNodeList"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileNodeList (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileNodeList)
- description and source-code
```javascript
compileNodeList = function (node, frame) {
    this._compileChildren(node, frame);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileNot"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileNot (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileNot)
- description and source-code
```javascript
compileNot = function (node, frame) {
    this.emit('!');
    this.compile(node.target, frame);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileOr"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileOr (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileOr)
- description and source-code
```javascript
compileOr = function (node, frame) {
    this.compile(node.left, frame);
    this.emit(str);
    this.compile(node.right, frame);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileOutput"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileOutput (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileOutput)
- description and source-code
```javascript
compileOutput = function (node, frame) {
    var children = node.children;
    for(var i=0, l=children.length; i<l; i++) {
        // TemplateData is a special case because it is never
        // autoescaped, so simply output it for optimization
        if(children[i] instanceof nodes.TemplateData) {
            if(children[i].value) {
                this.emit(this.buffer + ' += ');
                this.compileLiteral(children[i], frame);
                this.emitLine(';');
            }
        }
        else {
            this.emit(this.buffer + ' += runtime.suppressValue(');
            if(this.throwOnUndefined) {
                this.emit('runtime.ensureDefined(');
            }
            this.compile(children[i], frame);
            if(this.throwOnUndefined) {
                this.emit(',' + node.lineno + ',' + node.colno + ')');
            }
            this.emit(', env.opts.autoescape);\n');
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compilePair"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compilePair (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compilePair)
- description and source-code
```javascript
compilePair = function (node, frame) {
    var key = node.key;
    var val = node.value;

    if(key instanceof nodes.Symbol) {
        key = new nodes.Literal(key.lineno, key.colno, key.value);
    }
    else if(!(key instanceof nodes.Literal &&
              typeof key.value === 'string')) {
        this.fail('compilePair: Dict keys must be strings or names',
                  key.lineno,
                  key.colno);
    }

    this.compile(key, frame);
    this.emit(': ');
    this._compileExpression(val, frame);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compilePos"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compilePos (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compilePos)
- description and source-code
```javascript
compilePos = function (node, frame) {
    this.emit('+');
    this.compile(node.target, frame);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compilePow"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compilePow (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compilePow)
- description and source-code
```javascript
compilePow = function (node, frame) {
    this.emit('Math.pow(');
    this.compile(node.left, frame);
    this.emit(', ');
    this.compile(node.right, frame);
    this.emit(')');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileRoot"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileRoot (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileRoot)
- description and source-code
```javascript
compileRoot = function (node, frame) {
    if(frame) {
        this.fail('compileRoot: root node can\'t have frame');
    }

    frame = new Frame();

    this.emitFuncBegin('root');
    this.emitLine('var parentTemplate = null;');
    this._compileChildren(node, frame);
    this.emitLine('if(parentTemplate) {');
    this.emitLine('parentTemplate.rootRenderFunc(env, context, frame, runtime, cb);');
    this.emitLine('} else {');
    this.emitLine('cb(null, ' + this.buffer +');');
    this.emitLine('}');
    this.emitFuncEnd(true);

    this.inBlock = true;

    var blockNames = [];

    var i, name, block, blocks = node.findAll(nodes.Block);
    for (i = 0; i < blocks.length; i++) {
        block = blocks[i];
        name = block.name.value;

        if (blockNames.indexOf(name) !== -1) {
            throw new Error('Block "' + name + '" defined more than once.');
        }
        blockNames.push(name);

        this.emitFuncBegin('b_' + name);

        var tmpFrame = new Frame();
        this.emitLine('var frame = frame.push(true);');
        this.compile(block.body, tmpFrame);
        this.emitFuncEnd();
    }

    this.emitLine('return {');
    for (i = 0; i < blocks.length; i++) {
        block = blocks[i];
        name = 'b_' + block.name.value;
        this.emitLine(name + ': ' + name + ',');
    }
    this.emitLine('root: root\n};');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileSet"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileSet (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileSet)
- description and source-code
```javascript
compileSet = function (node, frame) {
    var ids = [];

    // Lookup the variable names for each identifier and create
    // new ones if necessary
    lib.each(node.targets, function(target) {
        var name = target.value;
        var id = frame.lookup(name);

        if (id === null || id === undefined) {
            id = this.tmpid();

            // Note: This relies on js allowing scope across
            // blocks, in case this is created inside an 'if'
            this.emitLine('var ' + id + ';');
        }

        ids.push(id);
    }, this);

    if (node.value) {
      this.emit(ids.join(' = ') + ' = ');
      this._compileExpression(node.value, frame);
      this.emitLine(';');
    }
    else {
      this.emit(ids.join(' = ') + ' = ');
      this.compile(node.body, frame);
      this.emitLine(';');
    }

    lib.each(node.targets, function(target, i) {
        var id = ids[i];
        var name = target.value;

        // We are running this for every var, but it's very
        // uncommon to assign to multiple vars anyway
        this.emitLine('frame.set("' + name + '", ' + id + ', true);');

        this.emitLine('if(frame.topLevel) {');
        this.emitLine('context.setVariable("' + name + '", ' + id + ');');
        this.emitLine('}');

        if(name.charAt(0) !== '_') {
            this.emitLine('if(frame.topLevel) {');
            this.emitLine('context.addExport("' + name + '", ' + id + ');');
            this.emitLine('}');
        }
    }, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileSub"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileSub (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileSub)
- description and source-code
```javascript
compileSub = function (node, frame) {
    this.compile(node.left, frame);
    this.emit(str);
    this.compile(node.right, frame);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileSuper"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileSuper (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileSuper)
- description and source-code
```javascript
compileSuper = function (node, frame) {
    var name = node.blockName.value;
    var id = node.symbol.value;

    this.emitLine('context.getSuper(env, ' +
                  '"' + name + '", ' +
                  'b_' + name + ', ' +
                  'frame, runtime, '+
                  this.makeCallback(id));
    this.emitLine(id + ' = runtime.markSafe(' + id + ');');
    this.addScopeLevel();
    frame.set(id, id);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileSymbol"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileSymbol (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileSymbol)
- description and source-code
```javascript
compileSymbol = function (node, frame) {
    var name = node.value;
    var v;

    if((v = frame.lookup(name))) {
        this.emit(v);
    }
    else {
        this.emit('runtime.contextOrFrameLookup(' +
                  'context, frame, "' + name + '")');
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.compileTemplateData"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>compileTemplateData (node, frame)](#apidoc.element.nunjucks.compiler.Compiler.prototype.compileTemplateData)
- description and source-code
```javascript
compileTemplateData = function (node, frame) {
    this.compileLiteral(node, frame);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>constructor ()](#apidoc.element.nunjucks.compiler.Compiler.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.emit"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>emit (code)](#apidoc.element.nunjucks.compiler.Compiler.prototype.emit)
- description and source-code
```javascript
emit = function (code) {
    this.codebuf.push(code);
}
```
- example usage
```shell
...
	    '>=': '>='
	};

	// A common pattern is to emit binary operators
	function binOpEmitter(str) {
	    return function(node, frame) {
	        this.compile(node.left, frame);
	        this.emit(str);
	        this.compile(node.right, frame);
	    };
	}

	var Compiler = Object.extend({
	    init: function(templateName, throwOnUndefined) {
	        this.templateName = templateName;
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.emitFuncBegin"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>emitFuncBegin (name)](#apidoc.element.nunjucks.compiler.Compiler.prototype.emitFuncBegin)
- description and source-code
```javascript
emitFuncBegin = function (name) {
    this.buffer = 'output';
    this.scopeClosers = '';
    this.emitLine('function ' + name + '(env, context, frame, runtime, cb) {');
    this.emitLine('var lineno = null;');
    this.emitLine('var colno = null;');
    this.emitLine('var ' + this.buffer + ' = "";');
    this.emitLine('try {');
}
```
- example usage
```shell
...
	    compileRoot: function(node, frame) {
	        if(frame) {
	            this.fail('compileRoot: root node can\'t have frame');
	        }

	        frame = new Frame();

	        this.emitFuncBegin('root');
	        this.emitLine('var parentTemplate = null;');
	        this._compileChildren(node, frame);
	        this.emitLine('if(parentTemplate) {');
	        this.emitLine('parentTemplate.rootRenderFunc(env, context, frame, runtime, cb);');
	        this.emitLine('} else {');
	        this.emitLine('cb(null, ' + this.buffer +');');
	        this.emitLine('}');
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.emitFuncEnd"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>emitFuncEnd (noReturn)](#apidoc.element.nunjucks.compiler.Compiler.prototype.emitFuncEnd)
- description and source-code
```javascript
emitFuncEnd = function (noReturn) {
    if(!noReturn) {
        this.emitLine('cb(null, ' + this.buffer +');');
    }

    this.closeScopeLevels();
    this.emitLine('} catch (e) {');
    this.emitLine('  cb(runtime.handleError(e, lineno, colno));');
    this.emitLine('}');
    this.emitLine('}');
    this.buffer = null;
}
```
- example usage
```shell
...
	        this.emitLine('var parentTemplate = null;');
	        this._compileChildren(node, frame);
	        this.emitLine('if(parentTemplate) {');
	        this.emitLine('parentTemplate.rootRenderFunc(env, context, frame, runtime, cb);');
	        this.emitLine('} else {');
	        this.emitLine('cb(null, ' + this.buffer +');');
	        this.emitLine('}');
	        this.emitFuncEnd(true);

	        this.inBlock = true;

	        var blockNames = [];

	        var i, name, block, blocks = node.findAll(nodes.Block);
	        for (i = 0; i < blocks.length; i++) {
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.emitLine"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>emitLine (code)](#apidoc.element.nunjucks.compiler.Compiler.prototype.emitLine)
- description and source-code
```javascript
emitLine = function (code) {
    this.emit(code + '\n');
}
```
- example usage
```shell
...

	    emitLine: function(code) {
	        this.emit(code + '\n');
	    },

	    emitLines: function() {
	        lib.each(lib.toArray(arguments), function(line) {
	            this.emitLine(line);
	        }, this);
	    },

	    emitFuncBegin: function(name) {
	        this.buffer = 'output';
	        this.scopeClosers = '';
	        this.emitLine('function ' + name + '(env, context, frame, runtime, cb) {');
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.emitLines"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>emitLines ()](#apidoc.element.nunjucks.compiler.Compiler.prototype.emitLines)
- description and source-code
```javascript
emitLines = function () {
    lib.each(lib.toArray(arguments), function(line) {
        this.emitLine(line);
    }, this);
}
```
- example usage
```shell
...
	                                 function(n) { return '"' + n.key.value + '"'; });

	        // We pass a function to makeMacro which destructures the
	        // arguments so support setting positional args with keywords
	        // args and passing keyword args as positional args
	        // (essentially default values). See runtime.js.
	        var frame = new Frame();
	        this.emitLines(
	            'var ' + funcId + ' = runtime.makeMacro(',
	            '[' + argNames.join(', ') + '], ',
	            '[' + kwargNames.join(', ') + '], ',
	            'function (' + realNames.join(', ') + ') {',
	            'var callerFrame = frame;',
	            'frame = new runtime.Frame();',
	            'kwargs = kwargs || {};',
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.emitLoopBindings"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>emitLoopBindings (node, arr, i, len)](#apidoc.element.nunjucks.compiler.Compiler.prototype.emitLoopBindings)
- description and source-code
```javascript
emitLoopBindings = function (node, arr, i, len) {
    var bindings = {
        index: i + ' + 1',
        index0: i,
        revindex: len + ' - ' + i,
        revindex0: len + ' - ' + i + ' - 1',
        first: i + ' === 0',
        last: i + ' === ' + len + ' - 1',
        length: len
    };

    for (var name in bindings) {
        this.emitLine('frame.set("loop.' + name + '", ' + bindings[name] + ');');
    }
}
```
- example usage
```shell
...
	                    var tid = this.tmpid();
	                    this.emitLine('var ' + tid + ' = ' + arr + '[' + i + '][' + u + ']');
	                    this.emitLine('frame.set("' + node.name.children[u].value
	                                  + '", ' + arr + '[' + i + '][' + u + ']' + ');');
	                    frame.set(node.name.children[u].value, tid);
	                }

	                this.emitLoopBindings(node, arr, i, len);
	                this.withScopedSyntax(function() {
	                    this.compile(node.body, frame);
	                });
	                this.emitLine('}');
	            }

	            this.emitLine('} else {'); {
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.fail"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>fail (msg, lineno, colno)](#apidoc.element.nunjucks.compiler.Compiler.prototype.fail)
- description and source-code
```javascript
fail = function (msg, lineno, colno) {
    if (lineno !== undefined) lineno += 1;
    if (colno !== undefined) colno += 1;

    throw new lib.TemplateError(msg, lineno, colno);
}
```
- example usage
```shell
...
	        for(var i=0; i<types.length; i++) {
	            if(node instanceof types[i]) {
	                success = true;
	            }
	        }

	        if(!success) {
	            this.fail('assertType: invalid type: ' + node.typename,
	                      node.lineno,
	                      node.colno);
	        }
	    },

	    compileCallExtension: function(node, frame, async) {
	        var args = node.args;
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.getCode"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>getCode ()](#apidoc.element.nunjucks.compiler.Compiler.prototype.getCode)
- description and source-code
```javascript
getCode = function () {
    return this.codebuf.join('');
}
```
- example usage
```shell
...
	// var c = new Compiler();
	// var src = 'hello {% filter title %}' +
	//     'Hello madam how are you' +
	//     '{% endfilter %}'
	// var ast = transformer.transform(parser.parse(src));
	// nodes.printNodes(ast);
	// c.compile(ast);
	// var tmpl = c.getCode();
	// console.log(tmpl);

	module.exports = {
	    compile: function(src, asyncFilters, extensions, name, opts) {
	        var c = new Compiler(name, opts.throwOnUndefined);

	        // Run the extension preprocessors against the source.
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.init"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>init (templateName, throwOnUndefined)](#apidoc.element.nunjucks.compiler.Compiler.prototype.init)
- description and source-code
```javascript
init = function (templateName, throwOnUndefined) {
    this.templateName = templateName;
    this.codebuf = [];
    this.lastId = 0;
    this.buffer = null;
    this.bufferStack = [];
    this.scopeClosers = '';
    this.inBlock = false;
    this.throwOnUndefined = throwOnUndefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.makeCallback"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>makeCallback (res)](#apidoc.element.nunjucks.compiler.Compiler.prototype.makeCallback)
- description and source-code
```javascript
makeCallback = function (res) {
    var err = this.tmpid();

    return 'function(' + err + (res ? ',' + res : '') + ') {\n' +
        'if(' + err + ') { cb(' + err + '); return; }';
}
```
- example usage
```shell
...
	                    this.emit('null');
	                }
	            }, this);
	        }

	        if(async) {
	            var res = this.tmpid();
	            this.emitLine(', ' + this.makeCallback(res));
	            this.emitLine(this.buffer + ' += runtime.suppressValue(' + res + ', ' + autoescape + ' && env.opts.autoescape);');
	            this.addScopeLevel();
	        }
	        else {
	            this.emit(')');
	            this.emit(', ' + autoescape + ' && env.opts.autoescape);\n');
	        }
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.popBufferId"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>popBufferId ()](#apidoc.element.nunjucks.compiler.Compiler.prototype.popBufferId)
- description and source-code
```javascript
popBufferId = function () {
    this.buffer = this.bufferStack.pop();
}
```
- example usage
```shell
...
	                    this.pushBufferId(id);

	                    this.withScopedSyntax(function() {
	                        this.compile(arg, frame);
	                        this.emitLine('cb(null, ' + id + ');');
	                    });

	                    this.popBufferId();
	                    this.emitLine('return ' + id + ';');
	                    this.emitLine('}');
	                }
	                else {
	                    this.emit('null');
	                }
	            }, this);
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.pushBufferId"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>pushBufferId (id)](#apidoc.element.nunjucks.compiler.Compiler.prototype.pushBufferId)
- description and source-code
```javascript
pushBufferId = function (id) {
    this.bufferStack.push(this.buffer);
    this.buffer = id;
    this.emit('var ' + this.buffer + ' = "";');
}
```
- example usage
```shell
...
	                }

	                if(arg) {
	                    var id = this.tmpid();

	                    this.emitLine('function(cb) {');
	                    this.emitLine('if(!cb) { cb = function(err) { if(err) { throw err; }}}');
	                    this.pushBufferId(id);

	                    this.withScopedSyntax(function() {
	                        this.compile(arg, frame);
	                        this.emitLine('cb(null, ' + id + ');');
	                    });

	                    this.popBufferId();
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.tmpid"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>tmpid ()](#apidoc.element.nunjucks.compiler.Compiler.prototype.tmpid)
- description and source-code
```javascript
tmpid = function () {
    this.lastId++;
    return 't_' + this.lastId;
}
```
- example usage
```shell
...
	        func.call(this);

	        this.closeScopeLevels();
	        this.scopeClosers = scopeClosers;
	    },

	    makeCallback: function(res) {
	        var err = this.tmpid();

	        return 'function(' + err + (res ? ',' + res : '') + ') {\n' +
	            'if(' + err + ') { cb(' + err + '); return; }';
	    },

	    tmpid: function() {
	        this.lastId++;
...
```

#### <a name="apidoc.element.nunjucks.compiler.Compiler.prototype.withScopedSyntax"></a>[function <span class="apidocSignatureSpan">nunjucks.compiler.Compiler.prototype.</span>withScopedSyntax (func)](#apidoc.element.nunjucks.compiler.Compiler.prototype.withScopedSyntax)
- description and source-code
```javascript
withScopedSyntax = function (func) {
    var scopeClosers = this.scopeClosers;
    this.scopeClosers = '';

    func.call(this);

    this.closeScopeLevels();
    this.scopeClosers = scopeClosers;
}
```
- example usage
```shell
...
	                if(arg) {
	                    var id = this.tmpid();

	                    this.emitLine('function(cb) {');
	                    this.emitLine('if(!cb) { cb = function(err) { if(err) { throw err; }}}');
	                    this.pushBufferId(id);

	                    this.withScopedSyntax(function() {
	                        this.compile(arg, frame);
	                        this.emitLine('cb(null, ' + id + ');');
	                    });

	                    this.popBufferId();
	                    this.emitLine('return ' + id + ';');
	                    this.emitLine('}');
...
```



# <a name="apidoc.module.nunjucks.environment"></a>[module nunjucks.environment](#apidoc.module.nunjucks.environment)

#### <a name="apidoc.element.nunjucks.environment.Environment"></a>[function <span class="apidocSignatureSpan">nunjucks.environment.</span>Environment ()](#apidoc.element.nunjucks.environment.Environment)
- description and source-code
```javascript
Environment = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
    else if(loaders.WebLoader) {
        TemplateLoader = new loaders.WebLoader(templatesPath, {
            useCache: opts.web && opts.web.useCache,
            async: opts.web && opts.web.async
        });
    }

    e = new env.Environment(TemplateLoader, opts);

    if(opts && opts.express) {
        e.express(opts.express);
    }

    return e;
};
...
```

#### <a name="apidoc.element.nunjucks.environment.Template"></a>[function <span class="apidocSignatureSpan">nunjucks.environment.</span>Template ()](#apidoc.element.nunjucks.environment.Template)
- description and source-code
```javascript
Template = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
return e;
};

module.exports.compile = function(src, env, path, eagerCompile) {
if(!e) {
    module.exports.configure();
}
return new module.exports.Template(src, env, path, eagerCompile);
};

module.exports.render = function(name, ctx, cb) {
if(!e) {
    module.exports.configure();
}
...
```



# <a name="apidoc.module.nunjucks.filters"></a>[module nunjucks.filters](#apidoc.module.nunjucks.filters)

#### <a name="apidoc.element.nunjucks.filters.abs"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>abs (n)](#apidoc.element.nunjucks.filters.abs)
- description and source-code
```javascript
abs = function (n) {
    return Math.abs(n);
}
```
- example usage
```shell
...
	        return Array.prototype.indexOf.call(arr, searchElement, fromIndex);
	    } :
	    function (arr, searchElement, fromIndex) {
	        var length = this.length >>> 0; // Hack to convert object.length to a UInt32

	        fromIndex = +fromIndex || 0;

	        if(Math.abs(fromIndex) === Infinity) {
	            fromIndex = 0;
	        }

	        if(fromIndex < 0) {
	            fromIndex += length;
	            if (fromIndex < 0) {
	                fromIndex = 0;
...
```

#### <a name="apidoc.element.nunjucks.filters.batch"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>batch (arr, linecount, fill_with)](#apidoc.element.nunjucks.filters.batch)
- description and source-code
```javascript
batch = function (arr, linecount, fill_with) {
    var i;
    var res = [];
    var tmp = [];

    for(i = 0; i < arr.length; i++) {
        if(i % linecount === 0 && tmp.length) {
            res.push(tmp);
            tmp = [];
        }

        tmp.push(arr[i]);
    }

    if(tmp.length) {
        if(fill_with) {
            for(i = tmp.length; i < linecount; i++) {
                tmp.push(fill_with);
            }
        }

        res.push(tmp);
    }

    return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.capitalize"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>capitalize (str)](#apidoc.element.nunjucks.filters.capitalize)
- description and source-code
```javascript
capitalize = function (str) {
    str = normalize(str, '');
    var ret = str.toLowerCase();
    return r.copySafeness(str, ret.charAt(0).toUpperCase() + ret.slice(1));
}
```
- example usage
```shell
...
	        return r.copySafeness(input, res);
	    },

	    title: function(str) {
	        str = normalize(str, '');
	        var words = str.split(' ');
	        for(var i = 0; i < words.length; i++) {
	            words[i] = filters.capitalize(words[i]);
	        }
	        return r.copySafeness(str, words.join(' '));
	    },

	    trim: function(str) {
	        return r.copySafeness(str, str.replace(/^\s*|\s*$/g, ''));
	    },
...
```

#### <a name="apidoc.element.nunjucks.filters.center"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>center (str, width)](#apidoc.element.nunjucks.filters.center)
- description and source-code
```javascript
center = function (str, width) {
    str = normalize(str, '');
    width = width || 80;

    if(str.length >= width) {
        return str;
    }

    var spaces = width - str.length;
    var pre = lib.repeat(' ', spaces/2 - spaces % 2);
    var post = lib.repeat(' ', spaces/2);
    return r.copySafeness(str, pre + str + post);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.d"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>d (val, def, bool)](#apidoc.element.nunjucks.filters.d)
- description and source-code
```javascript
d = function (val, def, bool) {
    if(bool) {
        return val ? val : def;
    }
    else {
        return (val !== undefined) ? val : def;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.default"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>default (val, def, bool)](#apidoc.element.nunjucks.filters.default)
- description and source-code
```javascript
default = function (val, def, bool) {
    if(bool) {
        return val ? val : def;
    }
    else {
        return (val !== undefined) ? val : def;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.dictsort"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>dictsort (val, case_sensitive, by)](#apidoc.element.nunjucks.filters.dictsort)
- description and source-code
```javascript
dictsort = function (val, case_sensitive, by) {
    if (!lib.isObject(val)) {
        throw new lib.TemplateError('dictsort filter: val must be an object');
    }

    var array = [];
    for (var k in val) {
        // deliberately include properties from the object's prototype
        array.push([k,val[k]]);
    }

    var si;
    if (by === undefined || by === 'key') {
        si = 0;
    } else if (by === 'value') {
        si = 1;
    } else {
        throw new lib.TemplateError(
            'dictsort filter: You can only sort by either key or value');
    }

    array.sort(function(t1, t2) {
        var a = t1[si];
        var b = t2[si];

        if (!case_sensitive) {
            if (lib.isString(a)) {
                a = a.toUpperCase();
            }
            if (lib.isString(b)) {
                b = b.toUpperCase();
            }
        }

        return a > b ? 1 : (a === b ? 0 : -1);
    });

    return array;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.dump"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>dump (obj, spaces)](#apidoc.element.nunjucks.filters.dump)
- description and source-code
```javascript
dump = function (obj, spaces) {
    return JSON.stringify(obj, null, spaces);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.e"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>e (str)](#apidoc.element.nunjucks.filters.e)
- description and source-code
```javascript
e = function (str) {
    if(str instanceof r.SafeString) {
        return str;
    }
    str = (str === null || str === undefined) ? '' : str;
    return r.markSafe(lib.escape(str.toString()));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.escape"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>escape (str)](#apidoc.element.nunjucks.filters.escape)
- description and source-code
```javascript
escape = function (str) {
    if(str instanceof r.SafeString) {
        return str;
    }
    str = (str === null || str === undefined) ? '' : str;
    return r.markSafe(lib.escape(str.toString()));
}
```
- example usage
```shell
...
	    },

	    escape: function(str) {
	        if(str instanceof r.SafeString) {
	            return str;
	        }
	        str = (str === null || str === undefined) ? '' : str;
	        return r.markSafe(lib.escape(str.toString()));
	    },

	    safe: function(str) {
	        if (str instanceof r.SafeString) {
	            return str;
	        }
	        str = (str === null || str === undefined) ? '' : str;
...
```

#### <a name="apidoc.element.nunjucks.filters.first"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>first (arr)](#apidoc.element.nunjucks.filters.first)
- description and source-code
```javascript
first = function (arr) {
    return arr[0];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.float"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>float (val, def)](#apidoc.element.nunjucks.filters.float)
- description and source-code
```javascript
float = function (val, def) {
    var res = parseFloat(val);
    return isNaN(res) ? def : res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.groupby"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>groupby (arr, attr)](#apidoc.element.nunjucks.filters.groupby)
- description and source-code
```javascript
groupby = function (arr, attr) {
    return lib.groupBy(arr, attr);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.indent"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>indent (str, width, indentfirst)](#apidoc.element.nunjucks.filters.indent)
- description and source-code
```javascript
indent = function (str, width, indentfirst) {
    str = normalize(str, '');

    if (str === '') return '';

    width = width || 4;
    var res = '';
    var lines = str.split('\n');
    var sp = lib.repeat(' ', width);

    for(var i=0; i<lines.length; i++) {
        if(i === 0 && !indentfirst) {
            res += lines[i] + '\n';
        }
        else {
            res += sp + lines[i] + '\n';
        }
    }

    return r.copySafeness(str, res);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.int"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>int (val, def)](#apidoc.element.nunjucks.filters.int)
- description and source-code
```javascript
int = function (val, def) {
    var res = parseInt(val, 10);
    return isNaN(res) ? def : res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.join"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>join (arr, del, attr)](#apidoc.element.nunjucks.filters.join)
- description and source-code
```javascript
join = function (arr, del, attr) {
    del = del || '';

    if(attr) {
        arr = lib.map(arr, function(v) {
            return v[attr];
        });
    }

    return arr.join(del);
}
```
- example usage
```shell
...

	        if(attr) {
	            arr = lib.map(arr, function(v) {
	                return v[attr];
	            });
	        }

	        return arr.join(del);
	    },

	    last: function(arr) {
	        return arr[arr.length-1];
	    },

	    length: function(val) {
...
```

#### <a name="apidoc.element.nunjucks.filters.last"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>last (arr)](#apidoc.element.nunjucks.filters.last)
- description and source-code
```javascript
last = function (arr) {
    return arr[arr.length-1];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.length"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>length (val)](#apidoc.element.nunjucks.filters.length)
- description and source-code
```javascript
length = function (val) {
    var value = normalize(val, '');

    if(value !== undefined) {
        if(
            (typeof Map === 'function' && value instanceof Map) ||
            (typeof Set === 'function' && value instanceof Set)
        ) {
            // ECMAScript 2015 Maps and Sets
            return value.size;
        }
        if(lib.isObject(value) && !(value instanceof r.SafeString)) {
            // Objects (besides SafeStrings), non-primative Arrays
            return Object.keys(value).length;
        }
        return value.length;
    }
    return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.list"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>list (val)](#apidoc.element.nunjucks.filters.list)
- description and source-code
```javascript
list = function (val) {
    if(lib.isString(val)) {
        return val.split('');
    }
    else if(lib.isObject(val)) {
        var keys = [];

        if(Object.keys) {
            keys = Object.keys(val);
        }
        else {
            for(var k in val) {
                keys.push(k);
            }
        }

        return lib.map(keys, function(k) {
            return { key: k,
                     value: val[k] };
        });
    }
    else if(lib.isArray(val)) {
      return val;
    }
    else {
        throw new lib.TemplateError('list filter: type not iterable');
    }
}
```
- example usage
```shell
...

	        return r.copySafeness(originalStr, res);
	    },

	    reverse: function(val) {
	        var arr;
	        if(lib.isString(val)) {
	            arr = filters.list(val);
	        }
	        else {
	            // Copy it
	            arr = lib.map(val, function(v) { return v; });
	        }

	        arr.reverse();
...
```

#### <a name="apidoc.element.nunjucks.filters.lower"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>lower (str)](#apidoc.element.nunjucks.filters.lower)
- description and source-code
```javascript
lower = function (str) {
    str = normalize(str, '');
    return str.toLowerCase();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.nl2br"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>nl2br (str)](#apidoc.element.nunjucks.filters.nl2br)
- description and source-code
```javascript
nl2br = function (str) {
    if (str === null || str === undefined) {
        return '';
    }
    return r.copySafeness(str, str.replace(/\r\n|\n/g, '<br />\n'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.random"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>random (arr)](#apidoc.element.nunjucks.filters.random)
- description and source-code
```javascript
random = function (arr) {
    return arr[Math.floor(Math.random() * arr.length)];
}
```
- example usage
```shell
...
	        if (str === null || str === undefined) {
	            return '';
	        }
	        return r.copySafeness(str, str.replace(/\r\n|\n/g, '<br />\n'));
	    },

	    random: function(arr) {
	        return arr[Math.floor(Math.random() * arr.length)];
	    },

	    rejectattr: function(arr, attr) {
	      return arr.filter(function (item) {
	        return !item[attr];
	      });
	    },
...
```

#### <a name="apidoc.element.nunjucks.filters.rejectattr"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>rejectattr (arr, attr)](#apidoc.element.nunjucks.filters.rejectattr)
- description and source-code
```javascript
rejectattr = function (arr, attr) {
  return arr.filter(function (item) {
    return !item[attr];
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.replace"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>replace (str, old, new_, maxCount)](#apidoc.element.nunjucks.filters.replace)
- description and source-code
```javascript
replace = function (str, old, new_, maxCount) {
    var originalStr = str;

    if (old instanceof RegExp) {
        return str.replace(old, new_);
    }

    if(typeof maxCount === 'undefined'){
        maxCount = -1;
    }

    var res = '';  // Output

    // Cast Numbers in the search term to string
    if(typeof old === 'number'){
        old = old + '';
    }
    else if(typeof old !== 'string') {
        // If it is something other than number or string,
        // return the original string
        return str;
    }

    // Cast numbers in the replacement to string
    if(typeof str === 'number'){
        str = str + '';
    }

    // If by now, we don't have a string, throw it back
    if(typeof str !== 'string' && !(str instanceof r.SafeString)){
        return str;
    }

    // ShortCircuits
    if(old === ''){
        // Mimic the python behaviour: empty string is replaced
        // by replacement e.g. "abc"|replace("", ".") -> .a.b.c.
        res = new_ + str.split('').join(new_) + new_;
        return r.copySafeness(str, res);
    }

    var nextIndex = str.indexOf(old);
    // if # of replacements to perform is 0, or the string to does
    // not contain the old value, return the string
    if(maxCount === 0 || nextIndex === -1){
        return str;
    }

    var pos = 0;
    var count = 0; // # of replacements made

    while(nextIndex  > -1 && (maxCount === -1 || count < maxCount)){
        // Grab the next chunk of src string and add it with the
        // replacement, to the result
        res += str.substring(pos, nextIndex) + new_;
        // Increment our pointer in the src string
        pos = nextIndex + old.length;
        count++;
        // See if there are any more replacements to be made
        nextIndex = str.indexOf(old, pos);
    }

    // We've either reached the end, or done the max # of
    // replacements, tack on any remaining string
    if(pos < str.length) {
        res += str.substring(pos);
    }

    return r.copySafeness(originalStr, res);
}
```
- example usage
```shell
...

	    return err;
	};

	exports.TemplateError.prototype = Error.prototype;

	exports.escape = function(val) {
	  return val.replace(escapeRegex, lookupEscape);
	};

	exports.isFunction = function(obj) {
	    return ObjProto.toString.call(obj) === '[object Function]';
	};

	exports.isArray = Array.isArray || function(obj) {
...
```

#### <a name="apidoc.element.nunjucks.filters.reverse"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>reverse (val)](#apidoc.element.nunjucks.filters.reverse)
- description and source-code
```javascript
reverse = function (val) {
    var arr;
    if(lib.isString(val)) {
        arr = filters.list(val);
    }
    else {
        // Copy it
        arr = lib.map(val, function(v) { return v; });
    }

    arr.reverse();

    if(lib.isString(val)) {
        return r.copySafeness(val, arr.join(''));
    }
    return arr;
}
```
- example usage
```shell
...
	            arr = filters.list(val);
	        }
	        else {
	            // Copy it
	            arr = lib.map(val, function(v) { return v; });
	        }

	        arr.reverse();

	        if(lib.isString(val)) {
	            return r.copySafeness(val, arr.join(''));
	        }
	        return arr;
	    },
...
```

#### <a name="apidoc.element.nunjucks.filters.round"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>round (val, precision, method)](#apidoc.element.nunjucks.filters.round)
- description and source-code
```javascript
round = function (val, precision, method) {
    precision = precision || 0;
    var factor = Math.pow(10, precision);
    var rounder;

    if(method === 'ceil') {
        rounder = Math.ceil;
    }
    else if(method === 'floor') {
        rounder = Math.floor;
    }
    else {
        rounder = Math.round;
    }

    return rounder(val * factor) / factor;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.safe"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>safe (str)](#apidoc.element.nunjucks.filters.safe)
- description and source-code
```javascript
safe = function (str) {
    if (str instanceof r.SafeString) {
        return str;
    }
    str = (str === null || str === undefined) ? '' : str;
    return r.markSafe(str.toString());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.selectattr"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>selectattr (arr, attr)](#apidoc.element.nunjucks.filters.selectattr)
- description and source-code
```javascript
selectattr = function (arr, attr) {
  return arr.filter(function (item) {
    return !!item[attr];
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.slice"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>slice (arr, slices, fillWith)](#apidoc.element.nunjucks.filters.slice)
- description and source-code
```javascript
slice = function (arr, slices, fillWith) {
    var sliceLength = Math.floor(arr.length / slices);
    var extra = arr.length % slices;
    var offset = 0;
    var res = [];

    for(var i=0; i<slices; i++) {
        var start = offset + i * sliceLength;
        if(i < extra) {
            offset++;
        }
        var end = offset + (i + 1) * sliceLength;

        var slice = arr.slice(start, end);
        if(fillWith && i >= extra) {
            slice.push(fillWith);
        }
        res.push(slice);
    }

    return res;
}
```
- example usage
```shell
...
	exports.without = function(array) {
	    var result = [];
	    if (!array) {
	        return result;
	    }
	    var index = -1,
	    length = array.length,
	    contains = exports.toArray(arguments).slice(1);

	    while(++index < length) {
	        if(exports.indexOf(contains, array[index]) === -1) {
	            result.push(array[index]);
	        }
	    }
	    return result;
...
```

#### <a name="apidoc.element.nunjucks.filters.sort"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>sort ()](#apidoc.element.nunjucks.filters.sort)
- description and source-code
```javascript
sort = function () {
    var argCount = numArgs(arguments);
    var args;
    var kwargs = getKeywordArgs(arguments);
    var i;

    if(argCount > argNames.length) {
        args = Array.prototype.slice.call(arguments, 0, argNames.length);

        // Positional arguments that should be passed in as
        // keyword arguments (essentially default values)
        var vals = Array.prototype.slice.call(arguments, args.length, argCount);
        for(i = 0; i < vals.length; i++) {
            if(i < kwargNames.length) {
                kwargs[kwargNames[i]] = vals[i];
            }
        }

        args.push(kwargs);
    }
    else if(argCount < argNames.length) {
        args = Array.prototype.slice.call(arguments, 0, argCount);

        for(i = argCount; i < argNames.length; i++) {
            var arg = argNames[i];

            // Keyword arguments that should be passed as
            // positional arguments, i.e. the caller explicitly
            // used the name of a positional arg
            args.push(kwargs[arg]);
            delete kwargs[arg];
        }

        args.push(kwargs);
    }
    else {
        args = arguments;
    }

    return func.apply(this, args);
}
```
- example usage
```shell
...
	        } else if (by === 'value') {
	            si = 1;
	        } else {
	            throw new lib.TemplateError(
	                'dictsort filter: You can only sort by either key or value');
	        }

	        array.sort(function(t1, t2) {
	            var a = t1[si];
	            var b = t2[si];

	            if (!case_sensitive) {
	                if (lib.isString(a)) {
	                    a = a.toUpperCase();
	                }
...
```

#### <a name="apidoc.element.nunjucks.filters.string"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>string (obj)](#apidoc.element.nunjucks.filters.string)
- description and source-code
```javascript
string = function (obj) {
    return r.copySafeness(obj, obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.striptags"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>striptags (input, preserve_linebreaks)](#apidoc.element.nunjucks.filters.striptags)
- description and source-code
```javascript
striptags = function (input, preserve_linebreaks) {
    input = normalize(input, '');
    preserve_linebreaks = preserve_linebreaks || false;
    var tags = /<\/?([a-z][a-z0-9]*)\b[^>]*>|<!--[\s\S]*?-->/gi;
    var trimmedInput = filters.trim(input.replace(tags, ''));
    var res = '';
    if (preserve_linebreaks) {
        res = trimmedInput
            .replace(/^ +| +$/gm, '')     // remove leading and trailing spaces
            .replace(/ +/g, ' ')          // squash adjacent spaces
            .replace(/(\r\n)/g, '\n')     // normalize linebreaks (CRLF -> LF)
            .replace(/\n\n\n+/g, '\n\n'); // squash abnormal adjacent linebreaks
    } else {
        res = trimmedInput.replace(/\s+/gi, ' ');
    }
    return r.copySafeness(input, res);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.sum"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>sum (arr, attr, start)](#apidoc.element.nunjucks.filters.sum)
- description and source-code
```javascript
sum = function (arr, attr, start) {
    var sum = 0;

    if(typeof start === 'number'){
        sum += start;
    }

    if(attr) {
        arr = lib.map(arr, function(v) {
            return v[attr];
        });
    }

    for(var i = 0; i < arr.length; i++) {
        sum += arr[i];
    }

    return sum;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.title"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>title (str)](#apidoc.element.nunjucks.filters.title)
- description and source-code
```javascript
title = function (str) {
    str = normalize(str, '');
    var words = str.split(' ');
    for(var i = 0; i < words.length; i++) {
        words[i] = filters.capitalize(words[i]);
    }
    return r.copySafeness(str, words.join(' '));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.trim"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>trim (str)](#apidoc.element.nunjucks.filters.trim)
- description and source-code
```javascript
trim = function (str) {
    return r.copySafeness(str, str.replace(/^\s*|\s*$/g, ''));
}
```
- example usage
```shell
...
	        return r.copySafeness(obj, obj);
	    },

	    striptags: function(input, preserve_linebreaks) {
	        input = normalize(input, '');
	        preserve_linebreaks = preserve_linebreaks || false;
	        var tags = /<\/?([a-z][a-z0-9]*)\b[^>]*>|<!--[\s\S]*?-->/gi;
	        var trimmedInput = filters.trim(input.replace(tags, ''));
	        var res = '';
	        if (preserve_linebreaks) {
	            res = trimmedInput
	                .replace(/^ +| +$/gm, '')     // remove leading and trailing spaces
	                .replace(/ +/g, ' ')          // squash adjacent spaces
	                .replace(/(\r\n)/g, '\n')     // normalize linebreaks (CRLF -> LF)
	                .replace(/\n\n\n+/g, '\n\n'); // squash abnormal adjacent linebreaks
...
```

#### <a name="apidoc.element.nunjucks.filters.truncate"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>truncate (input, length, killwords, end)](#apidoc.element.nunjucks.filters.truncate)
- description and source-code
```javascript
truncate = function (input, length, killwords, end) {
    var orig = input;
    input = normalize(input, '');
    length = length || 255;

    if (input.length <= length)
        return input;

    if (killwords) {
        input = input.substring(0, length);
    } else {
        var idx = input.lastIndexOf(' ', length);
        if(idx === -1) {
            idx = length;
        }

        input = input.substring(0, idx);
    }

    input += (end !== undefined && end !== null) ? end : '...';
    return r.copySafeness(orig, input);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.upper"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>upper (str)](#apidoc.element.nunjucks.filters.upper)
- description and source-code
```javascript
upper = function (str) {
    str = normalize(str, '');
    return str.toUpperCase();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.urlencode"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>urlencode (obj)](#apidoc.element.nunjucks.filters.urlencode)
- description and source-code
```javascript
urlencode = function (obj) {
    var enc = encodeURIComponent;
    if (lib.isString(obj)) {
        return enc(obj);
    } else {
        var parts;
        if (lib.isArray(obj)) {
            parts = obj.map(function(item) {
                return enc(item[0]) + '=' + enc(item[1]);
            });
        } else {
            parts = [];
            for (var k in obj) {
                if (obj.hasOwnProperty(k)) {
                    parts.push(enc(k) + '=' + enc(obj[k]));
                }
            }
        }
        return parts.join('&');
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.urlize"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>urlize (str, length, nofollow)](#apidoc.element.nunjucks.filters.urlize)
- description and source-code
```javascript
urlize = function (str, length, nofollow) {
    if (isNaN(length)) length = Infinity;

    var noFollowAttr = (nofollow === true ? ' rel="nofollow"' : '');

    // For the jinja regexp, see
    // https://github.com/mitsuhiko/jinja2/blob/f15b814dcba6aa12bc74d1f7d0c881d55f7126be/jinja2/utils.py#L20-L23
    var puncRE = /^(?:\(|<|&lt;)?(.*?)(?:\.|,|\)|\n|&gt;)?$/;
    // from http://blog.gerv.net/2011/05/html5_email_address_regexp/
    var emailRE = /^[\w.!#$%&'*+\-\/=?\^'{|}~]+@[a-z\d\-]+(\.[a-z\d\-]+)+$/i;
    var httpHttpsRE = /^https?:\/\/.*$/;
    var wwwRE = /^www\./;
    var tldRE = /\.(?:org|net|com)(?:\:|\/|$)/;

    var words = str.split(/(\s+)/).filter(function(word) {
      // If the word has no length, bail. This can happen for str with
      // trailing whitespace.
      return word && word.length;
    }).map(function(word) {
      var matches = word.match(puncRE);
      var possibleUrl = matches && matches[1] || word;

      // url that starts with http or https
      if (httpHttpsRE.test(possibleUrl))
        return '<a href="' + possibleUrl + '"' + noFollowAttr + '>' + possibleUrl.substr(0, length) + '</a>';

      // url that starts with www.
      if (wwwRE.test(possibleUrl))
        return '<a href="http://' + possibleUrl + '"' + noFollowAttr + '>' + possibleUrl.substr(0, length) + '</a>';

      // an email address of the form username@domain.tld
      if (emailRE.test(possibleUrl))
        return '<a href="mailto:' + possibleUrl + '">' + possibleUrl + '</a>';

      // url that ends in .com, .org or .net that is not an email address
      if (tldRE.test(possibleUrl))
        return '<a href="http://' + possibleUrl + '"' + noFollowAttr + '>' + possibleUrl.substr(0, length) + '</a>';

      return word;

    });

    return words.join('');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.filters.wordcount"></a>[function <span class="apidocSignatureSpan">nunjucks.filters.</span>wordcount (str)](#apidoc.element.nunjucks.filters.wordcount)
- description and source-code
```javascript
wordcount = function (str) {
    str = normalize(str, '');
    var words = (str) ? str.match(/\w+/g) : null;
    return (words) ? words.length : null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.lexer"></a>[module nunjucks.lexer](#apidoc.module.nunjucks.lexer)

#### <a name="apidoc.element.nunjucks.lexer.lex"></a>[function <span class="apidocSignatureSpan">nunjucks.lexer.</span>lex (src, opts)](#apidoc.element.nunjucks.lexer.lex)
- description and source-code
```javascript
lex = function (src, opts) {
    return new Tokenizer(src, opts);
}
```
- example usage
```shell
...
	    parseAsRoot: function() {
	        return new nodes.Root(0, 0, this.parseNodes());
	    }
	});

	// var util = require('util');

	// var l = lexer.lex('{%- if x -%}\n hello {% endif %}');
	// var t;
	// while((t = l.nextToken())) {
	//     console.log(util.inspect(t));
	// }

	// var p = new Parser(lexer.lex('hello {% filter title %}' +
	//                              'Hello madam how are you' +
...
```



# <a name="apidoc.module.nunjucks.lib"></a>[module nunjucks.lib](#apidoc.module.nunjucks.lib)

#### <a name="apidoc.element.nunjucks.lib.TemplateError"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>TemplateError (message, lineno, colno)](#apidoc.element.nunjucks.lib.TemplateError)
- description and source-code
```javascript
TemplateError = function (message, lineno, colno) {
    var err = this;

    if (message instanceof Error) { // for casting regular js errors
        err = message;
        message = message.name + ': ' + message.message;

        try {
            if(err.name = '') {}
        }
        catch(e) {
            // If we can't set the name of the error object in this
            // environment, don't use it
            err = this;
        }
    } else {
        if(Error.captureStackTrace) {
            Error.captureStackTrace(err);
        }
    }

    err.name = 'Template render error';
    err.message = message;
    err.lineno = lineno;
    err.colno = colno;
    err.firstUpdate = true;

    err.Update = function(path) {
        var message = '(' + (path || 'unknown path') + ')';

        // only show lineno + colno next to path of template
        // where error occurred
        if (this.firstUpdate) {
            if(this.lineno && this.colno) {
                message += ' [Line ' + this.lineno + ', Column ' + this.colno + ']';
            }
            else if(this.lineno) {
                message += ' [Line ' + this.lineno + ']';
            }
        }

        message += '\n ';
        if (this.firstUpdate) {
            message += ' ';
        }

        this.message = message + (this.message || '');
        this.firstUpdate = false;
        return this;
    };

    return err;
}
```
- example usage
```shell
...
	var exports = module.exports = {};

	exports.prettifyError = function(path, withInternals, err) {
	    // jshint -W022
	    // http://jslinterrors.com/do-not-assign-to-the-exception-parameter
	    if (!err.Update) {
	        // not one of ours, cast it
	        err = new exports.TemplateError(err);
	    }
	    err.Update(path);

	    // Unless they marked the dev flag, show them a trace from here
	    if (!withInternals) {
	        var old = err;
	        err = new Error(old.message);
...
```

#### <a name="apidoc.element.nunjucks.lib.asyncFor"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>asyncFor (obj, iter, cb)](#apidoc.element.nunjucks.lib.asyncFor)
- description and source-code
```javascript
asyncFor = function (obj, iter, cb) {
    var keys = exports.keys(obj);
    var len = keys.length;
    var i = -1;

    function next() {
        i++;
        var k = keys[i];

        if(i < len) {
            iter(k, obj[k], i, len, next);
        }
        else {
            cb();
        }
    }

    next();
}
```
- example usage
```shell
...
	            default:
	                item.push(i, next);
	                iter.apply(this, item);
	            }
	        }, cb);
	    }
	    else {
	        lib.asyncFor(arr, function(key, val, i, len, next) {
	            iter(key, val, i, len, next);
	        }, cb);
	    }
	}

	function asyncAll(arr, dimen, func, cb) {
	    var finished = 0;
...
```

#### <a name="apidoc.element.nunjucks.lib.asyncIter"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>asyncIter (arr, iter, cb)](#apidoc.element.nunjucks.lib.asyncIter)
- description and source-code
```javascript
asyncIter = function (arr, iter, cb) {
    var i = -1;

    function next() {
        i++;

        if(i < arr.length) {
            iter(arr[i], i, next, cb);
        }
        else {
            cb();
        }
    }

    next();
}
```
- example usage
```shell
...
	                    }
	                    else {
	                        syncResult = tmpl;
	                    }
	                }
	            };

	            lib.asyncIter(this.loaders, function(loader, i, next, done) {
	                function handle(err, src) {
	                    if(err) {
	                        done(err);
	                    }
	                    else if(src) {
	                        src.loader = loader;
	                        done(null, src);
...
```

#### <a name="apidoc.element.nunjucks.lib.each"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>each (obj, func, context)](#apidoc.element.nunjucks.lib.each)
- description and source-code
```javascript
each = function (obj, func, context) {
    if(obj == null) {
        return;
    }

    if(ArrayProto.each && obj.each === ArrayProto.each) {
        obj.forEach(func, context);
    }
    else if(obj.length === +obj.length) {
        for(var i=0, l=obj.length; i<l; i++) {
            func.call(context, obj[i], i, obj);
        }
    }
}
```
- example usage
```shell
...
	        for(var name in builtin_filters) {
	            this.addFilter(name, builtin_filters[name]);
	        }
	    },

	    initCache: function() {
	        // Caching and cache busting
	        lib.each(this.loaders, function(loader) {
	            loader.cache = {};

	            if(typeof loader.on === 'function') {
	                loader.on('update', function(template) {
	                    loader.cache[template] = null;
	                });
	            }
...
```

#### <a name="apidoc.element.nunjucks.lib.escape"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>escape (val)](#apidoc.element.nunjucks.lib.escape)
- description and source-code
```javascript
escape = function (val) {
  return val.replace(escapeRegex, lookupEscape);
}
```
- example usage
```shell
...
	    },

	    escape: function(str) {
	        if(str instanceof r.SafeString) {
	            return str;
	        }
	        str = (str === null || str === undefined) ? '' : str;
	        return r.markSafe(lib.escape(str.toString()));
	    },

	    safe: function(str) {
	        if (str instanceof r.SafeString) {
	            return str;
	        }
	        str = (str === null || str === undefined) ? '' : str;
...
```

#### <a name="apidoc.element.nunjucks.lib.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>extend (obj, obj2)](#apidoc.element.nunjucks.lib.extend)
- description and source-code
```javascript
extend = function (obj, obj2) {
    for(var k in obj2) {
        obj[k] = obj2[k];
    }
    return obj;
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```

#### <a name="apidoc.element.nunjucks.lib.groupBy"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>groupBy (obj, val)](#apidoc.element.nunjucks.lib.groupBy)
- description and source-code
```javascript
groupBy = function (obj, val) {
    var result = {};
    var iterator = exports.isFunction(val) ? val : function(obj) { return obj[val]; };
    for(var i=0; i<obj.length; i++) {
        var value = obj[i];
        var key = iterator(value, i);
        (result[key] || (result[key] = [])).push(value);
    }
    return result;
}
```
- example usage
```shell
...
	    },

	    first: function(arr) {
	        return arr[0];
	    },

	    groupby: function(arr, attr) {
	        return lib.groupBy(arr, attr);
	    },

	    indent: function(str, width, indentfirst) {
	        str = normalize(str, '');

	        if (str === '') return '';
...
```

#### <a name="apidoc.element.nunjucks.lib.inOperator"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>inOperator (key, val)](#apidoc.element.nunjucks.lib.inOperator)
- description and source-code
```javascript
inOperator = function (key, val) {
    if (exports.isArray(val)) {
        return exports.indexOf(val, key) !== -1;
    } else if (exports.isObject(val)) {
        return key in val;
    } else if (exports.isString(val)) {
        return val.indexOf(key) !== -1;
    } else {
        throw new Error('Cannot use "in" operator to search for "'
            + key + '" in unexpected types.');
    }
}
```
- example usage
```shell
...
	            this.compile(node.else_, frame);
	        else
	            this.emit('""');
	        this.emit(')');
	    },

	    compileIn: function(node, frame) {
	      this.emit('runtime.inOperator(');
	      this.compile(node.left, frame);
	      this.emit(',');
	      this.compile(node.right, frame);
	      this.emit(')');
	    },

	    compileOr: binOpEmitter(' || '),
...
```

#### <a name="apidoc.element.nunjucks.lib.indexOf"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>indexOf (arr, searchElement, fromIndex)](#apidoc.element.nunjucks.lib.indexOf)
- description and source-code
```javascript
indexOf = function (arr, searchElement, fromIndex) {
    return Array.prototype.indexOf.call(arr, searchElement, fromIndex);
}
```
- example usage
```shell
...
	        return result;
	    }
	    var index = -1,
	    length = array.length,
	    contains = exports.toArray(arguments).slice(1);

	    while(++index < length) {
	        if(exports.indexOf(contains, array[index]) === -1) {
	            result.push(array[index]);
	        }
	    }
	    return result;
	};

	exports.extend = function(obj, obj2) {
...
```

#### <a name="apidoc.element.nunjucks.lib.isArray"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>isArray ()](#apidoc.element.nunjucks.lib.isArray)
- description and source-code
```javascript
function isArray() { [native code] }
```
- example usage
```shell
...
	            }
	        }
	        return keys;
	    }
	};

	exports.inOperator = function (key, val) {
	    if (exports.isArray(val)) {
	        return exports.indexOf(val, key) !== -1;
	    } else if (exports.isObject(val)) {
	        return key in val;
	    } else if (exports.isString(val)) {
	        return val.indexOf(key) !== -1;
	    } else {
	        throw new Error('Cannot use "in" operator to search for "'
...
```

#### <a name="apidoc.element.nunjucks.lib.isFunction"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>isFunction (obj)](#apidoc.element.nunjucks.lib.isFunction)
- description and source-code
```javascript
isFunction = function (obj) {
    return ObjProto.toString.call(obj) === '[object Function]';
}
```
- example usage
```shell
...

	exports.isObject = function(obj) {
	    return ObjProto.toString.call(obj) === '[object Object]';
	};

	exports.groupBy = function(obj, val) {
	    var result = {};
	    var iterator = exports.isFunction(val) ? val : function(obj) { return obj[val]; };
	    for(var i=0; i<obj.length; i++) {
	        var value = obj[i];
	        var key = iterator(value, i);
	        (result[key] || (result[key] = [])).push(value);
	    }
	    return result;
	};
...
```

#### <a name="apidoc.element.nunjucks.lib.isObject"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>isObject (obj)](#apidoc.element.nunjucks.lib.isObject)
- description and source-code
```javascript
isObject = function (obj) {
    return ObjProto.toString.call(obj) === '[object Object]';
}
```
- example usage
```shell
...
module.exports.installJinjaCompat = require('./src/jinja-compat.js');

// A single instance of an environment, since this is so commonly used

var e;
module.exports.configure = function(templatesPath, opts) {
opts = opts || {};
if(lib.isObject(templatesPath)) {
    opts = templatesPath;
    templatesPath = null;
}

var TemplateLoader;
if(loaders.FileSystemLoader) {
    TemplateLoader = new loaders.FileSystemLoader(templatesPath, {
...
```

#### <a name="apidoc.element.nunjucks.lib.isString"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>isString (obj)](#apidoc.element.nunjucks.lib.isString)
- description and source-code
```javascript
isString = function (obj) {
    return ObjProto.toString.call(obj) === '[object String]';
}
```
- example usage
```shell
...
	};

	exports.inOperator = function (key, val) {
	    if (exports.isArray(val)) {
	        return exports.indexOf(val, key) !== -1;
	    } else if (exports.isObject(val)) {
	        return key in val;
	    } else if (exports.isString(val)) {
	        return val.indexOf(key) !== -1;
	    } else {
	        throw new Error('Cannot use "in" operator to search for "'
	            + key + '" in unexpected types.');
	    }
	};
...
```

#### <a name="apidoc.element.nunjucks.lib.keys"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>keys (obj)](#apidoc.element.nunjucks.lib.keys)
- description and source-code
```javascript
keys = function (obj) {
    if(Object.prototype.keys) {
        return obj.keys();
    }
    else {
        var keys = [];
        for(var k in obj) {
            if(obj.hasOwnProperty(k)) {
                keys.push(k);
            }
        }
        return keys;
    }
}
```
- example usage
```shell
...
	        }
	    }

	    next();
	};

	exports.asyncFor = function(obj, iter, cb) {
	    var keys = exports.keys(obj);
	    var len = keys.length;
	    var i = -1;

	    function next() {
	        i++;
	        var k = keys[i];
...
```

#### <a name="apidoc.element.nunjucks.lib.map"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>map (obj, func)](#apidoc.element.nunjucks.lib.map)
- description and source-code
```javascript
map = function (obj, func) {
    var results = [];
    if(obj == null) {
        return results;
    }

    if(ArrayProto.map && obj.map === ArrayProto.map) {
        return obj.map(func);
    }

    for(var i=0; i<obj.length; i++) {
        results[results.length] = func(obj[i], i);
    }

    if(obj.length === +obj.length) {
        results.length = obj.length;
    }

    return results;
}
```
- example usage
```shell
...
	exports.map = function(obj, func) {
	    var results = [];
	    if(obj == null) {
	        return results;
	    }

	    if(ArrayProto.map && obj.map === ArrayProto.map) {
	        return obj.map(func);
	    }

	    for(var i=0; i<obj.length; i++) {
	        results[results.length] = func(obj[i], i);
	    }

	    if(obj.length === +obj.length) {
...
```

#### <a name="apidoc.element.nunjucks.lib.prettifyError"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>prettifyError (path, withInternals, err)](#apidoc.element.nunjucks.lib.prettifyError)
- description and source-code
```javascript
prettifyError = function (path, withInternals, err) {
    // jshint -W022
    // http://jslinterrors.com/do-not-assign-to-the-exception-parameter
    if (!err.Update) {
        // not one of ours, cast it
        err = new exports.TemplateError(err);
    }
    err.Update(path);

    // Unless they marked the dev flag, show them a trace from here
    if (!withInternals) {
        var old = err;
        err = new Error(old.message);
        err.name = old.name;
    }

    return err;
}
```
- example usage
```shell
...

	        if(eagerCompile) {
	            var _this = this;
	            try {
	                _this._compile();
	            }
	            catch(err) {
	                throw lib.prettifyError(this.path, this.env.opts.dev, err);
	            }
	        }
	        else {
	            this.compiled = false;
	        }
	    },
...
```

#### <a name="apidoc.element.nunjucks.lib.repeat"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>repeat (char_, n)](#apidoc.element.nunjucks.lib.repeat)
- description and source-code
```javascript
repeat = function (char_, n) {
    var str = '';
    for(var i=0; i<n; i++) {
        str += char_;
    }
    return str;
}
```
- example usage
```shell
...
	        width = width || 80;

	        if(str.length >= width) {
	            return str;
	        }

	        var spaces = width - str.length;
	        var pre = lib.repeat(' ', spaces/2 - spaces % 2);
	        var post = lib.repeat(' ', spaces/2);
	        return r.copySafeness(str, pre + str + post);
	    },

	    'default': function(val, def, bool) {
	        if(bool) {
	            return val ? val : def;
...
```

#### <a name="apidoc.element.nunjucks.lib.toArray"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>toArray (obj)](#apidoc.element.nunjucks.lib.toArray)
- description and source-code
```javascript
toArray = function (obj) {
    return Array.prototype.slice.call(obj);
}
```
- example usage
```shell
...
	exports.without = function(array) {
	    var result = [];
	    if (!array) {
	        return result;
	    }
	    var index = -1,
	    length = array.length,
	    contains = exports.toArray(arguments).slice(1);

	    while(++index < length) {
	        if(exports.indexOf(contains, array[index]) === -1) {
	            result.push(array[index]);
	        }
	    }
	    return result;
...
```

#### <a name="apidoc.element.nunjucks.lib.without"></a>[function <span class="apidocSignatureSpan">nunjucks.lib.</span>without (array)](#apidoc.element.nunjucks.lib.without)
- description and source-code
```javascript
without = function (array) {
    var result = [];
    if (!array) {
        return result;
    }
    var index = -1,
    length = array.length,
    contains = exports.toArray(arguments).slice(1);

    while(++index < length) {
        if(exports.indexOf(contains, array[index]) === -1) {
            result.push(array[index]);
        }
    }
    return result;
}
```
- example usage
```shell
...
	        return this;
	    },

	    removeExtension: function(name) {
	        var extension = this.getExtension(name);
	        if (!extension) return;

	        this.extensionsList = lib.without(this.extensionsList, extension);
	        delete this.extensions[name];
	    },

	    getExtension: function(name) {
	        return this.extensions[name];
	    },
...
```



# <a name="apidoc.module.nunjucks.loaders"></a>[module nunjucks.loaders](#apidoc.module.nunjucks.loaders)

#### <a name="apidoc.element.nunjucks.loaders.FileSystemLoader"></a>[function <span class="apidocSignatureSpan">nunjucks.loaders.</span>FileSystemLoader ()](#apidoc.element.nunjucks.loaders.FileSystemLoader)
- description and source-code
```javascript
FileSystemLoader = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
if(lib.isObject(templatesPath)) {
    opts = templatesPath;
    templatesPath = null;
}

var TemplateLoader;
if(loaders.FileSystemLoader) {
    TemplateLoader = new loaders.FileSystemLoader(templatesPath, {
        watch: opts.watch,
        noCache: opts.noCache
    });
}
else if(loaders.WebLoader) {
    TemplateLoader = new loaders.WebLoader(templatesPath, {
        useCache: opts.web && opts.web.useCache,
...
```

#### <a name="apidoc.element.nunjucks.loaders.PrecompiledLoader"></a>[function <span class="apidocSignatureSpan">nunjucks.loaders.</span>PrecompiledLoader ()](#apidoc.element.nunjucks.loaders.PrecompiledLoader)
- description and source-code
```javascript
PrecompiledLoader = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        }

	        // It's easy to use precompiled templates: just include them
	        // before you configure nunjucks and this will automatically
	        // pick it up and use it
	        if((true) && window.nunjucksPrecompiled) {
	            this.loaders.unshift(
	                new builtin_loaders.PrecompiledLoader(window.nunjucksPrecompiled)
	            );
	        }

	        this.initCache();

	        this.globals = globals();
	        this.filters = {};
...
```



# <a name="apidoc.module.nunjucks.nodes"></a>[module nunjucks.nodes](#apidoc.module.nunjucks.nodes)

#### <a name="apidoc.element.nunjucks.nodes.Add"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Add ()](#apidoc.element.nunjucks.nodes.Add)
- description and source-code
```javascript
Add = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parseAdd: function() {
	        var node = this.parseSub();
	        while(this.skipValue(lexer.TOKEN_OPERATOR, '+')) {
	            var node2 = this.parseSub();
	            node = new nodes.Add(node.lineno,
	                                 node.colno,
	                                 node,
	                                 node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.And"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>And ()](#apidoc.element.nunjucks.nodes.And)
- description and source-code
```javascript
And = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parseAnd: function() {
	        var node = this.parseNot();
	        while(this.skipSymbol('and')) {
	            var node2 = this.parseNot();
	            node = new nodes.And(node.lineno,
	                                 node.colno,
	                                 node,
	                                 node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.Array"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Array ()](#apidoc.element.nunjucks.nodes.Array)
- description and source-code
```javascript
Array = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	            this.fail('parseFor: variable name expected for loop');
	        }

	        var type = this.peekToken().type;
	        if(type === lexer.TOKEN_COMMA) {
	            // key/value iteration
	            var key = node.name;
	            node.name = new nodes.Array(key.lineno, key.colno);
	            node.name.addChild(key);

	            while(this.skip(lexer.TOKEN_COMMA)) {
	                var prim = this.parsePrimary();
	                node.name.addChild(prim);
	            }
	        }
...
```

#### <a name="apidoc.element.nunjucks.nodes.AsyncAll"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>AsyncAll ()](#apidoc.element.nunjucks.nodes.AsyncAll)
- description and source-code
```javascript
AsyncAll = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	            endBlock = 'endfor';
	        }
	        else if(this.skipSymbol('asyncEach')) {
	            node = new nodes.AsyncEach(forTok.lineno, forTok.colno);
	            endBlock = 'endeach';
	        }
	        else if(this.skipSymbol('asyncAll')) {
	            node = new nodes.AsyncAll(forTok.lineno, forTok.colno);
	            endBlock = 'endall';
	        }
	        else {
	            this.fail('parseFor: expected for{Async}', forTok.lineno, forTok.colno);
	        }

	        node.name = this.parsePrimary();
...
```

#### <a name="apidoc.element.nunjucks.nodes.AsyncEach"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>AsyncEach ()](#apidoc.element.nunjucks.nodes.AsyncEach)
- description and source-code
```javascript
AsyncEach = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        var endBlock;

	        if(this.skipSymbol('for')) {
	            node = new nodes.For(forTok.lineno, forTok.colno);
	            endBlock = 'endfor';
	        }
	        else if(this.skipSymbol('asyncEach')) {
	            node = new nodes.AsyncEach(forTok.lineno, forTok.colno);
	            endBlock = 'endeach';
	        }
	        else if(this.skipSymbol('asyncAll')) {
	            node = new nodes.AsyncAll(forTok.lineno, forTok.colno);
	            endBlock = 'endall';
	        }
	        else {
...
```

#### <a name="apidoc.element.nunjucks.nodes.BinOp"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>BinOp ()](#apidoc.element.nunjucks.nodes.BinOp)
- description and source-code
```javascript
BinOp = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Block"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Block ()](#apidoc.element.nunjucks.nodes.Block)
- description and source-code
```javascript
Block = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...

	    parseBlock: function() {
	        var tag = this.peekToken();
	        if(!this.skipSymbol('block')) {
	            this.fail('parseBlock: expected block', tag.lineno, tag.colno);
	        }

	        var node = new nodes.Block(tag.lineno, tag.colno);

	        node.name = this.parsePrimary();
	        if(!(node.name instanceof nodes.Symbol)) {
	            this.fail('parseBlock: variable name expected',
	                      tag.lineno,
	                      tag.colno);
	        }
...
```

#### <a name="apidoc.element.nunjucks.nodes.CallExtension"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>CallExtension ()](#apidoc.element.nunjucks.nodes.CallExtension)
- description and source-code
```javascript
CallExtension = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.CallExtensionAsync"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>CallExtensionAsync ()](#apidoc.element.nunjucks.nodes.CallExtensionAsync)
- description and source-code
```javascript
CallExtensionAsync = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Caller"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Caller ()](#apidoc.element.nunjucks.nodes.Caller)
- description and source-code
```javascript
Caller = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        this.advanceAfterBlockEnd(callTok.value);
	        var body = this.parseUntilBlocks('endcall');
	        this.advanceAfterBlockEnd();

	        var callerName = new nodes.Symbol(callTok.lineno,
	                                          callTok.colno,
	                                          'caller');
	        var callerNode = new nodes.Caller(callTok.lineno,
	                                          callTok.colno,
	                                          callerName,
	                                          callerArgs,
	                                          body);

	        // add the additional caller kwarg, adding kwargs if necessary
	        var args = macroCall.args.children;
...
```

#### <a name="apidoc.element.nunjucks.nodes.Capture"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Capture ()](#apidoc.element.nunjucks.nodes.Capture)
- description and source-code
```javascript
Capture = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        if(!this.skipValue(lexer.TOKEN_OPERATOR, '=')) {
	            if (!this.skip(lexer.TOKEN_BLOCK_END)) {
	                this.fail('parseSet: expected = or block end in set tag',
	                          tag.lineno,
	                          tag.colno);
	            }
	            else {
	                node.body = new nodes.Capture(
	                    tag.lineno,
	                    tag.colno,
	                    this.parseUntilBlocks('endset')
	                );
	                node.value = null;
	                this.advanceAfterBlockEnd();
	            }
...
```

#### <a name="apidoc.element.nunjucks.nodes.Compare"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Compare ()](#apidoc.element.nunjucks.nodes.Compare)
- description and source-code
```javascript
Compare = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	            else {
	                this.pushToken(tok);
	                break;
	            }
	        }

	        if(ops.length) {
	            return new nodes.Compare(ops[0].lineno,
	                                     ops[0].colno,
	                                     expr,
	                                     ops);
	        }
	        else {
	            return expr;
	        }
...
```

#### <a name="apidoc.element.nunjucks.nodes.CompareOperand"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>CompareOperand ()](#apidoc.element.nunjucks.nodes.CompareOperand)
- description and source-code
```javascript
CompareOperand = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        while(1) {
	            var tok = this.nextToken();

	            if(!tok) {
	                break;
	            }
	            else if(lib.indexOf(compareOps, tok.value) !== -1) {
	                ops.push(new nodes.CompareOperand(tok.lineno,
	                                                  tok.colno,
	                                                  this.parseConcat(),
	                                                  tok.value));
	            }
	            else {
	                this.pushToken(tok);
	                break;
...
```

#### <a name="apidoc.element.nunjucks.nodes.Concat"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Concat ()](#apidoc.element.nunjucks.nodes.Concat)
- description and source-code
```javascript
Concat = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	    },

	    // finds the '~' for string concatenation
	    parseConcat: function(){
	        var node = this.parseAdd();
	        while(this.skipValue(lexer.TOKEN_TILDE, '~')) {
	            var node2 = this.parseAdd();
	            node = new nodes.Concat(node.lineno,
	                                 node.colno,
	                                 node,
	                                 node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.Dict"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Dict ()](#apidoc.element.nunjucks.nodes.Dict)
- description and source-code
```javascript
Dict = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...

	        switch(tok.type) {
	        case lexer.TOKEN_LEFT_PAREN:
	            node = new nodes.Group(tok.lineno, tok.colno); break;
	        case lexer.TOKEN_LEFT_BRACKET:
	            node = new nodes.Array(tok.lineno, tok.colno); break;
	        case lexer.TOKEN_LEFT_CURLY:
	            node = new nodes.Dict(tok.lineno, tok.colno); break;
	        default:
	            return null;
	        }

	        while(1) {
	            var type = this.peekToken().type;
	            if(type === lexer.TOKEN_RIGHT_PAREN ||
...
```

#### <a name="apidoc.element.nunjucks.nodes.Div"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Div ()](#apidoc.element.nunjucks.nodes.Div)
- description and source-code
```javascript
Div = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parseDiv: function() {
	        var node = this.parseFloorDiv();
	        while(this.skipValue(lexer.TOKEN_OPERATOR, '/')) {
	            var node2 = this.parseFloorDiv();
	            node = new nodes.Div(node.lineno,
	                                 node.colno,
	                                 node,
	                                 node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.Extends"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Extends ()](#apidoc.element.nunjucks.nodes.Extends)
- description and source-code
```javascript
Extends = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	    parseExtends: function() {
	        var tagName = 'extends';
	        var tag = this.peekToken();
	        if(!this.skipSymbol(tagName)) {
	            this.fail('parseTemplateRef: expected '+ tagName);
	        }

	        var node = new nodes.Extends(tag.lineno, tag.colno);
	        node.template = this.parseExpression();

	        this.advanceAfterBlockEnd(tag.value);
	        return node;
	    },

	    parseInclude: function() {
...
```

#### <a name="apidoc.element.nunjucks.nodes.Filter"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Filter ()](#apidoc.element.nunjucks.nodes.Filter)
- description and source-code
```javascript
Filter = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return [];
	    },

	    parseFilter: function(node) {
	        while(this.skip(lexer.TOKEN_PIPE)) {
	            var name = this.parseFilterName();

	            node = new nodes.Filter(
	                name.lineno,
	                name.colno,
	                name,
	                new nodes.NodeList(
	                    name.lineno,
	                    name.colno,
	                    [node].concat(this.parseFilterArgs(node))
...
```

#### <a name="apidoc.element.nunjucks.nodes.FilterAsync"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>FilterAsync ()](#apidoc.element.nunjucks.nodes.FilterAsync)
- description and source-code
```javascript
FilterAsync = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        else if((node instanceof nodes.Filter &&
	                 lib.indexOf(asyncFilters, node.name.value) !== -1) ||
	                node instanceof nodes.CallExtensionAsync) {
	            var symbol = new nodes.Symbol(node.lineno,
	                                          node.colno,
	                                          gensym());

	            children.push(new nodes.FilterAsync(node.lineno,
	                                                node.colno,
	                                                node.name,
	                                                node.args,
	                                                symbol));
	            return symbol;
	        }
	    });
...
```

#### <a name="apidoc.element.nunjucks.nodes.FloorDiv"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>FloorDiv ()](#apidoc.element.nunjucks.nodes.FloorDiv)
- description and source-code
```javascript
FloorDiv = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parseFloorDiv: function() {
	        var node = this.parseMod();
	        while(this.skipValue(lexer.TOKEN_OPERATOR, '//')) {
	            var node2 = this.parseMod();
	            node = new nodes.FloorDiv(node.lineno,
	                                      node.colno,
	                                      node,
	                                      node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.For"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>For ()](#apidoc.element.nunjucks.nodes.For)
- description and source-code
```javascript
For = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...

	    parseFor: function() {
	        var forTok = this.peekToken();
	        var node;
	        var endBlock;

	        if(this.skipSymbol('for')) {
	            node = new nodes.For(forTok.lineno, forTok.colno);
	            endBlock = 'endfor';
	        }
	        else if(this.skipSymbol('asyncEach')) {
	            node = new nodes.AsyncEach(forTok.lineno, forTok.colno);
	            endBlock = 'endeach';
	        }
	        else if(this.skipSymbol('asyncAll')) {
...
```

#### <a name="apidoc.element.nunjucks.nodes.FromImport"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>FromImport ()](#apidoc.element.nunjucks.nodes.FromImport)
- description and source-code
```javascript
FromImport = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	            else {
	                names.addChild(name);
	            }

	            withContext = this.parseWithContext();
	        }

	        return new nodes.FromImport(fromTok.lineno,
	                                    fromTok.colno,
	                                    template,
	                                    names,
	                                    withContext);
	    },

	    parseBlock: function() {
...
```

#### <a name="apidoc.element.nunjucks.nodes.FunCall"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>FunCall ()](#apidoc.element.nunjucks.nodes.FunCall)
- description and source-code
```javascript
FunCall = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...

	    parsePostfix: function(node) {
	        var lookup, tok = this.peekToken();

	        while(tok) {
	            if(tok.type === lexer.TOKEN_LEFT_PAREN) {
	                // Function call
	                node = new nodes.FunCall(tok.lineno,
	                                         tok.colno,
	                                         node,
	                                         this.parseSignature());
	            }
	            else if(tok.type === lexer.TOKEN_LEFT_BRACKET) {
	                // Reference
	                lookup = this.parseAggregate();
...
```

#### <a name="apidoc.element.nunjucks.nodes.Group"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Group ()](#apidoc.element.nunjucks.nodes.Group)
- description and source-code
```javascript
Group = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...

	    parseAggregate: function() {
	        var tok = this.nextToken();
	        var node;

	        switch(tok.type) {
	        case lexer.TOKEN_LEFT_PAREN:
	            node = new nodes.Group(tok.lineno, tok.colno); break;
	        case lexer.TOKEN_LEFT_BRACKET:
	            node = new nodes.Array(tok.lineno, tok.colno); break;
	        case lexer.TOKEN_LEFT_CURLY:
	            node = new nodes.Dict(tok.lineno, tok.colno); break;
	        default:
	            return null;
	        }
...
```

#### <a name="apidoc.element.nunjucks.nodes.If"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>If ()](#apidoc.element.nunjucks.nodes.If)
- description and source-code
```javascript
If = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	    },

	    parseIf: function() {
	        var tag = this.peekToken();
	        var node;

	        if(this.skipSymbol('if') || this.skipSymbol('elif') || this.skipSymbol('elseif')) {
	            node = new nodes.If(tag.lineno, tag.colno);
	        }
	        else if(this.skipSymbol('ifAsync')) {
	            node = new nodes.IfAsync(tag.lineno, tag.colno);
	        }
	        else {
	            this.fail('parseIf: expected if, elif, or elseif',
	                      tag.lineno,
...
```

#### <a name="apidoc.element.nunjucks.nodes.IfAsync"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>IfAsync ()](#apidoc.element.nunjucks.nodes.IfAsync)
- description and source-code
```javascript
IfAsync = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        var tag = this.peekToken();
	        var node;

	        if(this.skipSymbol('if') || this.skipSymbol('elif') || this.skipSymbol('elseif')) {
	            node = new nodes.If(tag.lineno, tag.colno);
	        }
	        else if(this.skipSymbol('ifAsync')) {
	            node = new nodes.IfAsync(tag.lineno, tag.colno);
	        }
	        else {
	            this.fail('parseIf: expected if, elif, or elseif',
	                      tag.lineno,
	                      tag.colno);
	        }
...
```

#### <a name="apidoc.element.nunjucks.nodes.Import"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Import ()](#apidoc.element.nunjucks.nodes.Import)
- description and source-code
```javascript
Import = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	                            importTok.colno);
	        }

	        var target = this.parseExpression();

	        var withContext = this.parseWithContext();

	        var node = new nodes.Import(importTok.lineno,
	                                    importTok.colno,
	                                    template,
	                                    target,
	                                    withContext);

	        this.advanceAfterBlockEnd(importTok.value);
...
```

#### <a name="apidoc.element.nunjucks.nodes.In"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>In ()](#apidoc.element.nunjucks.nodes.In)
- description and source-code
```javascript
In = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        var tok = this.nextToken();
	        if (!tok) { break; }
	        var invert = tok.type === lexer.TOKEN_SYMBOL && tok.value === 'not';
	        // if it wasn't 'not', put it back
	        if (!invert) { this.pushToken(tok); }
	        if (this.skipSymbol('in')) {
	          var node2 = this.parseCompare();
	          node = new nodes.In(node.lineno,
	                              node.colno,
	                              node,
	                              node2);
	          if (invert) {
	            node = new nodes.Not(node.lineno,
	                                 node.colno,
	                                 node);
...
```

#### <a name="apidoc.element.nunjucks.nodes.Include"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Include ()](#apidoc.element.nunjucks.nodes.Include)
- description and source-code
```javascript
Include = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	    parseInclude: function() {
	        var tagName = 'include';
	        var tag = this.peekToken();
	        if(!this.skipSymbol(tagName)) {
	            this.fail('parseInclude: expected '+ tagName);
	        }

	        var node = new nodes.Include(tag.lineno, tag.colno);
	        node.template = this.parseExpression();

	        if(this.skipSymbol('ignore') && this.skipSymbol('missing')) {
	            node.ignoreMissing = true;
	        }

	        this.advanceAfterBlockEnd(tag.value);
...
```

#### <a name="apidoc.element.nunjucks.nodes.InlineIf"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>InlineIf ()](#apidoc.element.nunjucks.nodes.InlineIf)
- description and source-code
```javascript
InlineIf = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	    },

	    parseInlineIf: function() {
	        var node = this.parseOr();
	        if(this.skipSymbol('if')) {
	            var cond_node = this.parseOr();
	            var body_node = node;
	            node = new nodes.InlineIf(node.lineno, node.colno);
	            node.body = body_node;
	            node.cond = cond_node;
	            if(this.skipSymbol('else')) {
	                node.else_ = this.parseOr();
	            } else {
	                node.else_ = null;
	            }
...
```

#### <a name="apidoc.element.nunjucks.nodes.KeywordArgs"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>KeywordArgs ()](#apidoc.element.nunjucks.nodes.KeywordArgs)
- description and source-code
```javascript
KeywordArgs = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	                                          callerName,
	                                          callerArgs,
	                                          body);

	        // add the additional caller kwarg, adding kwargs if necessary
	        var args = macroCall.args.children;
	        if (!(args[args.length-1] instanceof nodes.KeywordArgs)) {
	          args.push(new nodes.KeywordArgs());
	        }
	        var kwargs = args[args.length - 1];
	        kwargs.addChild(new nodes.Pair(callTok.lineno,
	                                       callTok.colno,
	                                       callerName,
	                                       callerNode));
...
```

#### <a name="apidoc.element.nunjucks.nodes.Literal"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Literal ()](#apidoc.element.nunjucks.nodes.Literal)
- description and source-code
```javascript
Literal = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	    },

	    compilePair: function(node, frame) {
	        var key = node.key;
	        var val = node.value;

	        if(key instanceof nodes.Symbol) {
	            key = new nodes.Literal(key.lineno, key.colno, key.value);
	        }
	        else if(!(key instanceof nodes.Literal &&
	                  typeof key.value === 'string')) {
	            this.fail('compilePair: Dict keys must be strings or names',
	                      key.lineno,
	                      key.colno);
	        }
...
```

#### <a name="apidoc.element.nunjucks.nodes.LookupVal"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>LookupVal ()](#apidoc.element.nunjucks.nodes.LookupVal)
- description and source-code
```javascript
LookupVal = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	            else if(tok.type === lexer.TOKEN_LEFT_BRACKET) {
	                // Reference
	                lookup = this.parseAggregate();
	                if(lookup.children.length > 1) {
	                    this.fail('invalid index');
	                }

	                node =  new nodes.LookupVal(tok.lineno,
	                                            tok.colno,
	                                            node,
	                                            lookup.children[0]);
	            }
	            else if(tok.type === lexer.TOKEN_OPERATOR && tok.value === '.') {
	                // Reference
	                this.nextToken();
...
```

#### <a name="apidoc.element.nunjucks.nodes.Macro"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Macro ()](#apidoc.element.nunjucks.nodes.Macro)
- description and source-code
```javascript
Macro = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        var macroTok = this.peekToken();
	        if(!this.skipSymbol('macro')) {
	            this.fail('expected macro');
	        }

	        var name = this.parsePrimary(true);
	        var args = this.parseSignature();
	        var node = new nodes.Macro(macroTok.lineno,
	                                   macroTok.colno,
	                                   name,
	                                   args);

	        this.advanceAfterBlockEnd(macroTok.value);
	        node.body = this.parseUntilBlocks('endmacro');
	        this.advanceAfterBlockEnd();
...
```

#### <a name="apidoc.element.nunjucks.nodes.Mod"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Mod ()](#apidoc.element.nunjucks.nodes.Mod)
- description and source-code
```javascript
Mod = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parseMod: function() {
	        var node = this.parsePow();
	        while(this.skipValue(lexer.TOKEN_OPERATOR, '%')) {
	            var node2 = this.parsePow();
	            node = new nodes.Mod(node.lineno,
	                                 node.colno,
	                                 node,
	                                 node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.Mul"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Mul ()](#apidoc.element.nunjucks.nodes.Mul)
- description and source-code
```javascript
Mul = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parseMul: function() {
	        var node = this.parseDiv();
	        while(this.skipValue(lexer.TOKEN_OPERATOR, '*')) {
	            var node2 = this.parseDiv();
	            node = new nodes.Mul(node.lineno,
	                                 node.colno,
	                                 node,
	                                 node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.Neg"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Neg ()](#apidoc.element.nunjucks.nodes.Neg)
- description and source-code
```javascript
Neg = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	    },

	    parseUnary: function(noFilters) {
	        var tok = this.peekToken();
	        var node;

	        if(this.skipValue(lexer.TOKEN_OPERATOR, '-')) {
	            node = new nodes.Neg(tok.lineno,
	                                 tok.colno,
	                                 this.parseUnary(true));
	        }
	        else if(this.skipValue(lexer.TOKEN_OPERATOR, '+')) {
	            node = new nodes.Pos(tok.lineno,
	                                 tok.colno,
	                                 this.parseUnary(true));
...
```

#### <a name="apidoc.element.nunjucks.nodes.Node"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Node ()](#apidoc.element.nunjucks.nodes.Node)
- description and source-code
```javascript
Node = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.NodeList"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>NodeList ()](#apidoc.element.nunjucks.nodes.NodeList)
- description and source-code
```javascript
NodeList = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        // a call block is parsed as a normal FunCall, but with an added
	        // 'caller' kwarg which is a Caller node.
	        var callTok = this.peekToken();
	        if(!this.skipSymbol('call')) {
	            this.fail('expected call');
	        }

	        var callerArgs = this.parseSignature(true) || new nodes.NodeList();
	        var macroCall = this.parsePrimary();

	        this.advanceAfterBlockEnd(callTok.value);
	        var body = this.parseUntilBlocks('endcall');
	        this.advanceAfterBlockEnd();

	        var callerName = new nodes.Symbol(callTok.lineno,
...
```

#### <a name="apidoc.element.nunjucks.nodes.Not"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Not ()](#apidoc.element.nunjucks.nodes.Not)
- description and source-code
```javascript
Not = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        }
	        return node;
	    },

	    parseNot: function() {
	        var tok = this.peekToken();
	        if(this.skipSymbol('not')) {
	            return new nodes.Not(tok.lineno,
	                                 tok.colno,
	                                 this.parseNot());
	        }
	        return this.parseIn();
	    },

	    parseIn: function() {
...
```

#### <a name="apidoc.element.nunjucks.nodes.Or"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Or ()](#apidoc.element.nunjucks.nodes.Or)
- description and source-code
```javascript
Or = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parseOr: function() {
	        var node = this.parseAnd();
	        while(this.skipSymbol('or')) {
	            var node2 = this.parseAnd();
	            node = new nodes.Or(node.lineno,
	                                node.colno,
	                                node,
	                                node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.Output"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Output ()](#apidoc.element.nunjucks.nodes.Output)
- description and source-code
```javascript
Output = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        }
	        var kwargs = args[args.length - 1];
	        kwargs.addChild(new nodes.Pair(callTok.lineno,
	                                       callTok.colno,
	                                       callerName,
	                                       callerNode));

	        return new nodes.Output(callTok.lineno,
	                                callTok.colno,
	                                [macroCall]);
	    },

	    parseWithContext: function() {
	        var tok = this.peekToken();
...
```

#### <a name="apidoc.element.nunjucks.nodes.Pair"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Pair ()](#apidoc.element.nunjucks.nodes.Pair)
- description and source-code
```javascript
Pair = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...

	        // add the additional caller kwarg, adding kwargs if necessary
	        var args = macroCall.args.children;
	        if (!(args[args.length-1] instanceof nodes.KeywordArgs)) {
	          args.push(new nodes.KeywordArgs());
	        }
	        var kwargs = args[args.length - 1];
	        kwargs.addChild(new nodes.Pair(callTok.lineno,
	                                       callTok.colno,
	                                       callerName,
	                                       callerNode));

	        return new nodes.Output(callTok.lineno,
	                                callTok.colno,
	                                [macroCall]);
...
```

#### <a name="apidoc.element.nunjucks.nodes.Pos"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Pos ()](#apidoc.element.nunjucks.nodes.Pos)
- description and source-code
```javascript
Pos = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...

	        if(this.skipValue(lexer.TOKEN_OPERATOR, '-')) {
	            node = new nodes.Neg(tok.lineno,
	                                 tok.colno,
	                                 this.parseUnary(true));
	        }
	        else if(this.skipValue(lexer.TOKEN_OPERATOR, '+')) {
	            node = new nodes.Pos(tok.lineno,
	                                 tok.colno,
	                                 this.parseUnary(true));
	        }
	        else {
	            node = this.parsePrimary();
	        }
...
```

#### <a name="apidoc.element.nunjucks.nodes.Pow"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Pow ()](#apidoc.element.nunjucks.nodes.Pow)
- description and source-code
```javascript
Pow = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parsePow: function() {
	        var node = this.parseUnary();
	        while(this.skipValue(lexer.TOKEN_OPERATOR, '**')) {
	            var node2 = this.parseUnary();
	            node = new nodes.Pow(node.lineno,
	                                 node.colno,
	                                 node,
	                                 node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.Root"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Root ()](#apidoc.element.nunjucks.nodes.Root)
- description and source-code
```javascript
Root = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	    },

	    parse: function() {
	        return new nodes.NodeList(0, 0, this.parseNodes());
	    },

	    parseAsRoot: function() {
	        return new nodes.Root(0, 0, this.parseNodes());
	    }
	});

	// var util = require('util');

	// var l = lexer.lex('{%- if x -%}\n hello {% endif %}');
	// var t;
...
```

#### <a name="apidoc.element.nunjucks.nodes.Set"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Set ()](#apidoc.element.nunjucks.nodes.Set)
- description and source-code
```javascript
Set = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...

	    parseSet: function() {
	        var tag = this.peekToken();
	        if(!this.skipSymbol('set')) {
	            this.fail('parseSet: expected set', tag.lineno, tag.colno);
	        }

	        var node = new nodes.Set(tag.lineno, tag.colno, []);

	        var target;
	        while((target = this.parsePrimary())) {
	            node.targets.push(target);

	            if(!this.skip(lexer.TOKEN_COMMA)) {
	                break;
...
```

#### <a name="apidoc.element.nunjucks.nodes.Sub"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Sub ()](#apidoc.element.nunjucks.nodes.Sub)
- description and source-code
```javascript
Sub = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parseSub: function() {
	        var node = this.parseMul();
	        while(this.skipValue(lexer.TOKEN_OPERATOR, '-')) {
	            var node2 = this.parseMul();
	            node = new nodes.Sub(node.lineno,
	                                 node.colno,
	                                 node,
	                                 node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.Super"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Super ()](#apidoc.element.nunjucks.nodes.Super)
- description and source-code
```javascript
Super = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	               node.name.value === 'super') {
	                hasSuper = true;
	                return new nodes.Symbol(node.lineno, node.colno, symbol);
	            }
	        });

	        if(hasSuper) {
	            blockNode.body.children.unshift(new nodes.Super(
	                0, 0, blockNode.name, new nodes.Symbol(0, 0, symbol)
	            ));
	        }
	    });
	}

	function convertStatements(ast) {
...
```

#### <a name="apidoc.element.nunjucks.nodes.Symbol"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Symbol ()](#apidoc.element.nunjucks.nodes.Symbol)
- description and source-code
```javascript
Symbol = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        var callerArgs = this.parseSignature(true) || new nodes.NodeList();
	        var macroCall = this.parsePrimary();

	        this.advanceAfterBlockEnd(callTok.value);
	        var body = this.parseUntilBlocks('endcall');
	        this.advanceAfterBlockEnd();

	        var callerName = new nodes.Symbol(callTok.lineno,
	                                          callTok.colno,
	                                          'caller');
	        var callerNode = new nodes.Caller(callTok.lineno,
	                                          callTok.colno,
	                                          callerName,
	                                          callerArgs,
	                                          body);
...
```

#### <a name="apidoc.element.nunjucks.nodes.TemplateData"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>TemplateData ()](#apidoc.element.nunjucks.nodes.TemplateData)
- description and source-code
```javascript
TemplateData = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	                str += all;
	            }
	        }

	        return new nodes.Output(
	            begun.lineno,
	            begun.colno,
	            [new nodes.TemplateData(begun.lineno, begun.colno, str)]
	        );
	    },

	    parsePostfix: function(node) {
	        var lookup, tok = this.peekToken();

	        while(tok) {
...
```

#### <a name="apidoc.element.nunjucks.nodes.Value"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Value ()](#apidoc.element.nunjucks.nodes.Value)
- description and source-code
```javascript
Value = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.printNodes"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>printNodes (node, indent)](#apidoc.element.nunjucks.nodes.printNodes)
- description and source-code
```javascript
function printNodes(node, indent) {
    indent = indent || 0;

    // This is hacky, but this is just a debugging function anyway
    function print(str, indent, inline) {
        var lines = str.split('\n');

        for(var i=0; i<lines.length; i++) {
            if(lines[i]) {
                if((inline && i > 0) || !inline) {
                    for(var j=0; j<indent; j++) {
                        process.stdout.write(' ');
                    }
                }
            }

            if(i === lines.length-1) {
                process.stdout.write(lines[i]);
            }
            else {
                process.stdout.write(lines[i] + '\n');
            }
        }
    }

    print(node.typename + ': ', indent);

    if(node instanceof NodeList) {
        print('\n');
        lib.each(node.children, function(n) {
            printNodes(n, indent + 2);
        });
    }
    else if(node instanceof CallExtension) {
        print(node.extName + '.' + node.prop);
        print('\n');

        if(node.args) {
            printNodes(node.args, indent + 2);
        }

        if(node.contentArgs) {
            lib.each(node.contentArgs, function(n) {
                printNodes(n, indent + 2);
            });
        }
    }
    else {
        var nodes = null;
        var props = null;

        node.iterFields(function(val, field) {
            if(val instanceof Node) {
                nodes = nodes || {};
                nodes[field] = val;
            }
            else {
                props = props || {};
                props[field] = val;
            }
        });

        if(props) {
            print(JSON.stringify(props, null, 2) + '\n', null, true);
        }
        else {
            print('\n');
        }

        if(nodes) {
            for(var k in nodes) {
                printNodes(nodes[k], indent + 2);
            }
        }

    }
}
```
- example usage
```shell
...
	});

	// var c = new Compiler();
	// var src = 'hello {% filter title %}' +
	//     'Hello madam how are you' +
	//     '{% endfilter %}'
	// var ast = transformer.transform(parser.parse(src));
	// nodes.printNodes(ast);
	// c.compile(ast);
	// var tmpl = c.getCode();
	// console.log(tmpl);

	module.exports = {
	    compile: function(src, asyncFilters, extensions, name, opts) {
	        var c = new Compiler(name, opts.throwOnUndefined);
...
```



# <a name="apidoc.module.nunjucks.nodes.Add"></a>[module nunjucks.nodes.Add](#apidoc.module.nunjucks.nodes.Add)

#### <a name="apidoc.element.nunjucks.nodes.Add.Add"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Add ()](#apidoc.element.nunjucks.nodes.Add.Add)
- description and source-code
```javascript
Add = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parseAdd: function() {
	        var node = this.parseSub();
	        while(this.skipValue(lexer.TOKEN_OPERATOR, '+')) {
	            var node2 = this.parseSub();
	            node = new nodes.Add(node.lineno,
	                                 node.colno,
	                                 node,
	                                 node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.Add.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Add.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Add.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Add.prototype"></a>[module nunjucks.nodes.Add.prototype](#apidoc.module.nunjucks.nodes.Add.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Add.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Add.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Add.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.And"></a>[module nunjucks.nodes.And](#apidoc.module.nunjucks.nodes.And)

#### <a name="apidoc.element.nunjucks.nodes.And.And"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>And ()](#apidoc.element.nunjucks.nodes.And.And)
- description and source-code
```javascript
And = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parseAnd: function() {
	        var node = this.parseNot();
	        while(this.skipSymbol('and')) {
	            var node2 = this.parseNot();
	            node = new nodes.And(node.lineno,
	                                 node.colno,
	                                 node,
	                                 node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.And.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.And.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.And.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.And.prototype"></a>[module nunjucks.nodes.And.prototype](#apidoc.module.nunjucks.nodes.And.prototype)

#### <a name="apidoc.element.nunjucks.nodes.And.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.And.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.And.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Array"></a>[module nunjucks.nodes.Array](#apidoc.module.nunjucks.nodes.Array)

#### <a name="apidoc.element.nunjucks.nodes.Array.Array"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Array ()](#apidoc.element.nunjucks.nodes.Array.Array)
- description and source-code
```javascript
Array = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	            this.fail('parseFor: variable name expected for loop');
	        }

	        var type = this.peekToken().type;
	        if(type === lexer.TOKEN_COMMA) {
	            // key/value iteration
	            var key = node.name;
	            node.name = new nodes.Array(key.lineno, key.colno);
	            node.name.addChild(key);

	            while(this.skip(lexer.TOKEN_COMMA)) {
	                var prim = this.parsePrimary();
	                node.name.addChild(prim);
	            }
	        }
...
```

#### <a name="apidoc.element.nunjucks.nodes.Array.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Array.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Array.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Array.prototype"></a>[module nunjucks.nodes.Array.prototype](#apidoc.module.nunjucks.nodes.Array.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Array.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Array.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Array.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.AsyncAll"></a>[module nunjucks.nodes.AsyncAll](#apidoc.module.nunjucks.nodes.AsyncAll)

#### <a name="apidoc.element.nunjucks.nodes.AsyncAll.AsyncAll"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>AsyncAll ()](#apidoc.element.nunjucks.nodes.AsyncAll.AsyncAll)
- description and source-code
```javascript
AsyncAll = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	            endBlock = 'endfor';
	        }
	        else if(this.skipSymbol('asyncEach')) {
	            node = new nodes.AsyncEach(forTok.lineno, forTok.colno);
	            endBlock = 'endeach';
	        }
	        else if(this.skipSymbol('asyncAll')) {
	            node = new nodes.AsyncAll(forTok.lineno, forTok.colno);
	            endBlock = 'endall';
	        }
	        else {
	            this.fail('parseFor: expected for{Async}', forTok.lineno, forTok.colno);
	        }

	        node.name = this.parsePrimary();
...
```

#### <a name="apidoc.element.nunjucks.nodes.AsyncAll.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.AsyncAll.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.AsyncAll.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.AsyncAll.prototype"></a>[module nunjucks.nodes.AsyncAll.prototype](#apidoc.module.nunjucks.nodes.AsyncAll.prototype)

#### <a name="apidoc.element.nunjucks.nodes.AsyncAll.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.AsyncAll.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.AsyncAll.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.AsyncEach"></a>[module nunjucks.nodes.AsyncEach](#apidoc.module.nunjucks.nodes.AsyncEach)

#### <a name="apidoc.element.nunjucks.nodes.AsyncEach.AsyncEach"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>AsyncEach ()](#apidoc.element.nunjucks.nodes.AsyncEach.AsyncEach)
- description and source-code
```javascript
AsyncEach = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        var endBlock;

	        if(this.skipSymbol('for')) {
	            node = new nodes.For(forTok.lineno, forTok.colno);
	            endBlock = 'endfor';
	        }
	        else if(this.skipSymbol('asyncEach')) {
	            node = new nodes.AsyncEach(forTok.lineno, forTok.colno);
	            endBlock = 'endeach';
	        }
	        else if(this.skipSymbol('asyncAll')) {
	            node = new nodes.AsyncAll(forTok.lineno, forTok.colno);
	            endBlock = 'endall';
	        }
	        else {
...
```

#### <a name="apidoc.element.nunjucks.nodes.AsyncEach.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.AsyncEach.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.AsyncEach.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.AsyncEach.prototype"></a>[module nunjucks.nodes.AsyncEach.prototype](#apidoc.module.nunjucks.nodes.AsyncEach.prototype)

#### <a name="apidoc.element.nunjucks.nodes.AsyncEach.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.AsyncEach.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.AsyncEach.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.BinOp"></a>[module nunjucks.nodes.BinOp](#apidoc.module.nunjucks.nodes.BinOp)

#### <a name="apidoc.element.nunjucks.nodes.BinOp.BinOp"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>BinOp ()](#apidoc.element.nunjucks.nodes.BinOp.BinOp)
- description and source-code
```javascript
BinOp = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.BinOp.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.BinOp.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.BinOp.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.BinOp.prototype"></a>[module nunjucks.nodes.BinOp.prototype](#apidoc.module.nunjucks.nodes.BinOp.prototype)

#### <a name="apidoc.element.nunjucks.nodes.BinOp.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.BinOp.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.BinOp.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Block"></a>[module nunjucks.nodes.Block](#apidoc.module.nunjucks.nodes.Block)

#### <a name="apidoc.element.nunjucks.nodes.Block.Block"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Block ()](#apidoc.element.nunjucks.nodes.Block.Block)
- description and source-code
```javascript
Block = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...

	    parseBlock: function() {
	        var tag = this.peekToken();
	        if(!this.skipSymbol('block')) {
	            this.fail('parseBlock: expected block', tag.lineno, tag.colno);
	        }

	        var node = new nodes.Block(tag.lineno, tag.colno);

	        node.name = this.parsePrimary();
	        if(!(node.name instanceof nodes.Symbol)) {
	            this.fail('parseBlock: variable name expected',
	                      tag.lineno,
	                      tag.colno);
	        }
...
```

#### <a name="apidoc.element.nunjucks.nodes.Block.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Block.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Block.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Block.prototype"></a>[module nunjucks.nodes.Block.prototype](#apidoc.module.nunjucks.nodes.Block.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Block.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Block.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Block.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.CallExtension"></a>[module nunjucks.nodes.CallExtension](#apidoc.module.nunjucks.nodes.CallExtension)

#### <a name="apidoc.element.nunjucks.nodes.CallExtension.CallExtension"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>CallExtension ()](#apidoc.element.nunjucks.nodes.CallExtension.CallExtension)
- description and source-code
```javascript
CallExtension = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.CallExtension.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.CallExtension.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.CallExtension.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.CallExtension.prototype"></a>[module nunjucks.nodes.CallExtension.prototype](#apidoc.module.nunjucks.nodes.CallExtension.prototype)

#### <a name="apidoc.element.nunjucks.nodes.CallExtension.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.CallExtension.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.CallExtension.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.CallExtension.prototype.init"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.CallExtension.prototype.</span>init (ext, prop, args, contentArgs)](#apidoc.element.nunjucks.nodes.CallExtension.prototype.init)
- description and source-code
```javascript
init = function (ext, prop, args, contentArgs) {
    this.extName = ext._name || ext;
    this.prop = prop;
    this.args = args || new NodeList();
    this.contentArgs = contentArgs || [];
    this.autoescape = ext.autoescape;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.CallExtensionAsync"></a>[module nunjucks.nodes.CallExtensionAsync](#apidoc.module.nunjucks.nodes.CallExtensionAsync)

#### <a name="apidoc.element.nunjucks.nodes.CallExtensionAsync.CallExtensionAsync"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>CallExtensionAsync ()](#apidoc.element.nunjucks.nodes.CallExtensionAsync.CallExtensionAsync)
- description and source-code
```javascript
CallExtensionAsync = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.CallExtensionAsync.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.CallExtensionAsync.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.CallExtensionAsync.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.CallExtensionAsync.prototype"></a>[module nunjucks.nodes.CallExtensionAsync.prototype](#apidoc.module.nunjucks.nodes.CallExtensionAsync.prototype)

#### <a name="apidoc.element.nunjucks.nodes.CallExtensionAsync.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.CallExtensionAsync.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.CallExtensionAsync.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Caller"></a>[module nunjucks.nodes.Caller](#apidoc.module.nunjucks.nodes.Caller)

#### <a name="apidoc.element.nunjucks.nodes.Caller.Caller"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Caller ()](#apidoc.element.nunjucks.nodes.Caller.Caller)
- description and source-code
```javascript
Caller = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        this.advanceAfterBlockEnd(callTok.value);
	        var body = this.parseUntilBlocks('endcall');
	        this.advanceAfterBlockEnd();

	        var callerName = new nodes.Symbol(callTok.lineno,
	                                          callTok.colno,
	                                          'caller');
	        var callerNode = new nodes.Caller(callTok.lineno,
	                                          callTok.colno,
	                                          callerName,
	                                          callerArgs,
	                                          body);

	        // add the additional caller kwarg, adding kwargs if necessary
	        var args = macroCall.args.children;
...
```

#### <a name="apidoc.element.nunjucks.nodes.Caller.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Caller.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Caller.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Caller.prototype"></a>[module nunjucks.nodes.Caller.prototype](#apidoc.module.nunjucks.nodes.Caller.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Caller.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Caller.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Caller.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Capture"></a>[module nunjucks.nodes.Capture](#apidoc.module.nunjucks.nodes.Capture)

#### <a name="apidoc.element.nunjucks.nodes.Capture.Capture"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Capture ()](#apidoc.element.nunjucks.nodes.Capture.Capture)
- description and source-code
```javascript
Capture = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        if(!this.skipValue(lexer.TOKEN_OPERATOR, '=')) {
	            if (!this.skip(lexer.TOKEN_BLOCK_END)) {
	                this.fail('parseSet: expected = or block end in set tag',
	                          tag.lineno,
	                          tag.colno);
	            }
	            else {
	                node.body = new nodes.Capture(
	                    tag.lineno,
	                    tag.colno,
	                    this.parseUntilBlocks('endset')
	                );
	                node.value = null;
	                this.advanceAfterBlockEnd();
	            }
...
```

#### <a name="apidoc.element.nunjucks.nodes.Capture.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Capture.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Capture.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Capture.prototype"></a>[module nunjucks.nodes.Capture.prototype](#apidoc.module.nunjucks.nodes.Capture.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Capture.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Capture.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Capture.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Compare"></a>[module nunjucks.nodes.Compare](#apidoc.module.nunjucks.nodes.Compare)

#### <a name="apidoc.element.nunjucks.nodes.Compare.Compare"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Compare ()](#apidoc.element.nunjucks.nodes.Compare.Compare)
- description and source-code
```javascript
Compare = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	            else {
	                this.pushToken(tok);
	                break;
	            }
	        }

	        if(ops.length) {
	            return new nodes.Compare(ops[0].lineno,
	                                     ops[0].colno,
	                                     expr,
	                                     ops);
	        }
	        else {
	            return expr;
	        }
...
```

#### <a name="apidoc.element.nunjucks.nodes.Compare.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Compare.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Compare.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Compare.prototype"></a>[module nunjucks.nodes.Compare.prototype](#apidoc.module.nunjucks.nodes.Compare.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Compare.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Compare.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Compare.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.CompareOperand"></a>[module nunjucks.nodes.CompareOperand](#apidoc.module.nunjucks.nodes.CompareOperand)

#### <a name="apidoc.element.nunjucks.nodes.CompareOperand.CompareOperand"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>CompareOperand ()](#apidoc.element.nunjucks.nodes.CompareOperand.CompareOperand)
- description and source-code
```javascript
CompareOperand = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        while(1) {
	            var tok = this.nextToken();

	            if(!tok) {
	                break;
	            }
	            else if(lib.indexOf(compareOps, tok.value) !== -1) {
	                ops.push(new nodes.CompareOperand(tok.lineno,
	                                                  tok.colno,
	                                                  this.parseConcat(),
	                                                  tok.value));
	            }
	            else {
	                this.pushToken(tok);
	                break;
...
```

#### <a name="apidoc.element.nunjucks.nodes.CompareOperand.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.CompareOperand.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.CompareOperand.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.CompareOperand.prototype"></a>[module nunjucks.nodes.CompareOperand.prototype](#apidoc.module.nunjucks.nodes.CompareOperand.prototype)

#### <a name="apidoc.element.nunjucks.nodes.CompareOperand.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.CompareOperand.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.CompareOperand.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Concat"></a>[module nunjucks.nodes.Concat](#apidoc.module.nunjucks.nodes.Concat)

#### <a name="apidoc.element.nunjucks.nodes.Concat.Concat"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Concat ()](#apidoc.element.nunjucks.nodes.Concat.Concat)
- description and source-code
```javascript
Concat = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	    },

	    // finds the '~' for string concatenation
	    parseConcat: function(){
	        var node = this.parseAdd();
	        while(this.skipValue(lexer.TOKEN_TILDE, '~')) {
	            var node2 = this.parseAdd();
	            node = new nodes.Concat(node.lineno,
	                                 node.colno,
	                                 node,
	                                 node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.Concat.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Concat.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Concat.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Concat.prototype"></a>[module nunjucks.nodes.Concat.prototype](#apidoc.module.nunjucks.nodes.Concat.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Concat.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Concat.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Concat.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Dict"></a>[module nunjucks.nodes.Dict](#apidoc.module.nunjucks.nodes.Dict)

#### <a name="apidoc.element.nunjucks.nodes.Dict.Dict"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Dict ()](#apidoc.element.nunjucks.nodes.Dict.Dict)
- description and source-code
```javascript
Dict = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...

	        switch(tok.type) {
	        case lexer.TOKEN_LEFT_PAREN:
	            node = new nodes.Group(tok.lineno, tok.colno); break;
	        case lexer.TOKEN_LEFT_BRACKET:
	            node = new nodes.Array(tok.lineno, tok.colno); break;
	        case lexer.TOKEN_LEFT_CURLY:
	            node = new nodes.Dict(tok.lineno, tok.colno); break;
	        default:
	            return null;
	        }

	        while(1) {
	            var type = this.peekToken().type;
	            if(type === lexer.TOKEN_RIGHT_PAREN ||
...
```

#### <a name="apidoc.element.nunjucks.nodes.Dict.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Dict.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Dict.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Dict.prototype"></a>[module nunjucks.nodes.Dict.prototype](#apidoc.module.nunjucks.nodes.Dict.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Dict.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Dict.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Dict.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Div"></a>[module nunjucks.nodes.Div](#apidoc.module.nunjucks.nodes.Div)

#### <a name="apidoc.element.nunjucks.nodes.Div.Div"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Div ()](#apidoc.element.nunjucks.nodes.Div.Div)
- description and source-code
```javascript
Div = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parseDiv: function() {
	        var node = this.parseFloorDiv();
	        while(this.skipValue(lexer.TOKEN_OPERATOR, '/')) {
	            var node2 = this.parseFloorDiv();
	            node = new nodes.Div(node.lineno,
	                                 node.colno,
	                                 node,
	                                 node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.Div.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Div.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Div.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Div.prototype"></a>[module nunjucks.nodes.Div.prototype](#apidoc.module.nunjucks.nodes.Div.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Div.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Div.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Div.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Extends"></a>[module nunjucks.nodes.Extends](#apidoc.module.nunjucks.nodes.Extends)

#### <a name="apidoc.element.nunjucks.nodes.Extends.Extends"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Extends ()](#apidoc.element.nunjucks.nodes.Extends.Extends)
- description and source-code
```javascript
Extends = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	    parseExtends: function() {
	        var tagName = 'extends';
	        var tag = this.peekToken();
	        if(!this.skipSymbol(tagName)) {
	            this.fail('parseTemplateRef: expected '+ tagName);
	        }

	        var node = new nodes.Extends(tag.lineno, tag.colno);
	        node.template = this.parseExpression();

	        this.advanceAfterBlockEnd(tag.value);
	        return node;
	    },

	    parseInclude: function() {
...
```

#### <a name="apidoc.element.nunjucks.nodes.Extends.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Extends.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Extends.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Extends.prototype"></a>[module nunjucks.nodes.Extends.prototype](#apidoc.module.nunjucks.nodes.Extends.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Extends.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Extends.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Extends.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Filter"></a>[module nunjucks.nodes.Filter](#apidoc.module.nunjucks.nodes.Filter)

#### <a name="apidoc.element.nunjucks.nodes.Filter.Filter"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Filter ()](#apidoc.element.nunjucks.nodes.Filter.Filter)
- description and source-code
```javascript
Filter = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return [];
	    },

	    parseFilter: function(node) {
	        while(this.skip(lexer.TOKEN_PIPE)) {
	            var name = this.parseFilterName();

	            node = new nodes.Filter(
	                name.lineno,
	                name.colno,
	                name,
	                new nodes.NodeList(
	                    name.lineno,
	                    name.colno,
	                    [node].concat(this.parseFilterArgs(node))
...
```

#### <a name="apidoc.element.nunjucks.nodes.Filter.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Filter.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Filter.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Filter.prototype"></a>[module nunjucks.nodes.Filter.prototype](#apidoc.module.nunjucks.nodes.Filter.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Filter.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Filter.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Filter.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.FilterAsync"></a>[module nunjucks.nodes.FilterAsync](#apidoc.module.nunjucks.nodes.FilterAsync)

#### <a name="apidoc.element.nunjucks.nodes.FilterAsync.FilterAsync"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>FilterAsync ()](#apidoc.element.nunjucks.nodes.FilterAsync.FilterAsync)
- description and source-code
```javascript
FilterAsync = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        else if((node instanceof nodes.Filter &&
	                 lib.indexOf(asyncFilters, node.name.value) !== -1) ||
	                node instanceof nodes.CallExtensionAsync) {
	            var symbol = new nodes.Symbol(node.lineno,
	                                          node.colno,
	                                          gensym());

	            children.push(new nodes.FilterAsync(node.lineno,
	                                                node.colno,
	                                                node.name,
	                                                node.args,
	                                                symbol));
	            return symbol;
	        }
	    });
...
```

#### <a name="apidoc.element.nunjucks.nodes.FilterAsync.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.FilterAsync.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.FilterAsync.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.FilterAsync.prototype"></a>[module nunjucks.nodes.FilterAsync.prototype](#apidoc.module.nunjucks.nodes.FilterAsync.prototype)

#### <a name="apidoc.element.nunjucks.nodes.FilterAsync.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.FilterAsync.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.FilterAsync.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.FloorDiv"></a>[module nunjucks.nodes.FloorDiv](#apidoc.module.nunjucks.nodes.FloorDiv)

#### <a name="apidoc.element.nunjucks.nodes.FloorDiv.FloorDiv"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>FloorDiv ()](#apidoc.element.nunjucks.nodes.FloorDiv.FloorDiv)
- description and source-code
```javascript
FloorDiv = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parseFloorDiv: function() {
	        var node = this.parseMod();
	        while(this.skipValue(lexer.TOKEN_OPERATOR, '//')) {
	            var node2 = this.parseMod();
	            node = new nodes.FloorDiv(node.lineno,
	                                      node.colno,
	                                      node,
	                                      node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.FloorDiv.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.FloorDiv.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.FloorDiv.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.FloorDiv.prototype"></a>[module nunjucks.nodes.FloorDiv.prototype](#apidoc.module.nunjucks.nodes.FloorDiv.prototype)

#### <a name="apidoc.element.nunjucks.nodes.FloorDiv.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.FloorDiv.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.FloorDiv.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.For"></a>[module nunjucks.nodes.For](#apidoc.module.nunjucks.nodes.For)

#### <a name="apidoc.element.nunjucks.nodes.For.For"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>For ()](#apidoc.element.nunjucks.nodes.For.For)
- description and source-code
```javascript
For = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...

	    parseFor: function() {
	        var forTok = this.peekToken();
	        var node;
	        var endBlock;

	        if(this.skipSymbol('for')) {
	            node = new nodes.For(forTok.lineno, forTok.colno);
	            endBlock = 'endfor';
	        }
	        else if(this.skipSymbol('asyncEach')) {
	            node = new nodes.AsyncEach(forTok.lineno, forTok.colno);
	            endBlock = 'endeach';
	        }
	        else if(this.skipSymbol('asyncAll')) {
...
```

#### <a name="apidoc.element.nunjucks.nodes.For.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.For.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.For.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.For.prototype"></a>[module nunjucks.nodes.For.prototype](#apidoc.module.nunjucks.nodes.For.prototype)

#### <a name="apidoc.element.nunjucks.nodes.For.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.For.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.For.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.FromImport"></a>[module nunjucks.nodes.FromImport](#apidoc.module.nunjucks.nodes.FromImport)

#### <a name="apidoc.element.nunjucks.nodes.FromImport.FromImport"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>FromImport ()](#apidoc.element.nunjucks.nodes.FromImport.FromImport)
- description and source-code
```javascript
FromImport = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	            else {
	                names.addChild(name);
	            }

	            withContext = this.parseWithContext();
	        }

	        return new nodes.FromImport(fromTok.lineno,
	                                    fromTok.colno,
	                                    template,
	                                    names,
	                                    withContext);
	    },

	    parseBlock: function() {
...
```

#### <a name="apidoc.element.nunjucks.nodes.FromImport.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.FromImport.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.FromImport.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.FromImport.prototype"></a>[module nunjucks.nodes.FromImport.prototype](#apidoc.module.nunjucks.nodes.FromImport.prototype)

#### <a name="apidoc.element.nunjucks.nodes.FromImport.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.FromImport.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.FromImport.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.FromImport.prototype.init"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.FromImport.prototype.</span>init ()](#apidoc.element.nunjucks.nodes.FromImport.prototype.init)
- description and source-code
```javascript
init = function () {
    // Save the current parent method
    var tmp = this.parent;

    // Set parent to the previous method, call, and restore
    this.parent = parent;
    var res = src.apply(this, arguments);
    this.parent = tmp;

    return res;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.FunCall"></a>[module nunjucks.nodes.FunCall](#apidoc.module.nunjucks.nodes.FunCall)

#### <a name="apidoc.element.nunjucks.nodes.FunCall.FunCall"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>FunCall ()](#apidoc.element.nunjucks.nodes.FunCall.FunCall)
- description and source-code
```javascript
FunCall = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...

	    parsePostfix: function(node) {
	        var lookup, tok = this.peekToken();

	        while(tok) {
	            if(tok.type === lexer.TOKEN_LEFT_PAREN) {
	                // Function call
	                node = new nodes.FunCall(tok.lineno,
	                                         tok.colno,
	                                         node,
	                                         this.parseSignature());
	            }
	            else if(tok.type === lexer.TOKEN_LEFT_BRACKET) {
	                // Reference
	                lookup = this.parseAggregate();
...
```

#### <a name="apidoc.element.nunjucks.nodes.FunCall.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.FunCall.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.FunCall.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.FunCall.prototype"></a>[module nunjucks.nodes.FunCall.prototype](#apidoc.module.nunjucks.nodes.FunCall.prototype)

#### <a name="apidoc.element.nunjucks.nodes.FunCall.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.FunCall.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.FunCall.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Group"></a>[module nunjucks.nodes.Group](#apidoc.module.nunjucks.nodes.Group)

#### <a name="apidoc.element.nunjucks.nodes.Group.Group"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Group ()](#apidoc.element.nunjucks.nodes.Group.Group)
- description and source-code
```javascript
Group = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...

	    parseAggregate: function() {
	        var tok = this.nextToken();
	        var node;

	        switch(tok.type) {
	        case lexer.TOKEN_LEFT_PAREN:
	            node = new nodes.Group(tok.lineno, tok.colno); break;
	        case lexer.TOKEN_LEFT_BRACKET:
	            node = new nodes.Array(tok.lineno, tok.colno); break;
	        case lexer.TOKEN_LEFT_CURLY:
	            node = new nodes.Dict(tok.lineno, tok.colno); break;
	        default:
	            return null;
	        }
...
```

#### <a name="apidoc.element.nunjucks.nodes.Group.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Group.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Group.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Group.prototype"></a>[module nunjucks.nodes.Group.prototype](#apidoc.module.nunjucks.nodes.Group.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Group.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Group.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Group.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.If"></a>[module nunjucks.nodes.If](#apidoc.module.nunjucks.nodes.If)

#### <a name="apidoc.element.nunjucks.nodes.If.If"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>If ()](#apidoc.element.nunjucks.nodes.If.If)
- description and source-code
```javascript
If = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	    },

	    parseIf: function() {
	        var tag = this.peekToken();
	        var node;

	        if(this.skipSymbol('if') || this.skipSymbol('elif') || this.skipSymbol('elseif')) {
	            node = new nodes.If(tag.lineno, tag.colno);
	        }
	        else if(this.skipSymbol('ifAsync')) {
	            node = new nodes.IfAsync(tag.lineno, tag.colno);
	        }
	        else {
	            this.fail('parseIf: expected if, elif, or elseif',
	                      tag.lineno,
...
```

#### <a name="apidoc.element.nunjucks.nodes.If.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.If.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.If.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.If.prototype"></a>[module nunjucks.nodes.If.prototype](#apidoc.module.nunjucks.nodes.If.prototype)

#### <a name="apidoc.element.nunjucks.nodes.If.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.If.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.If.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.IfAsync"></a>[module nunjucks.nodes.IfAsync](#apidoc.module.nunjucks.nodes.IfAsync)

#### <a name="apidoc.element.nunjucks.nodes.IfAsync.IfAsync"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>IfAsync ()](#apidoc.element.nunjucks.nodes.IfAsync.IfAsync)
- description and source-code
```javascript
IfAsync = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        var tag = this.peekToken();
	        var node;

	        if(this.skipSymbol('if') || this.skipSymbol('elif') || this.skipSymbol('elseif')) {
	            node = new nodes.If(tag.lineno, tag.colno);
	        }
	        else if(this.skipSymbol('ifAsync')) {
	            node = new nodes.IfAsync(tag.lineno, tag.colno);
	        }
	        else {
	            this.fail('parseIf: expected if, elif, or elseif',
	                      tag.lineno,
	                      tag.colno);
	        }
...
```

#### <a name="apidoc.element.nunjucks.nodes.IfAsync.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.IfAsync.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.IfAsync.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.IfAsync.prototype"></a>[module nunjucks.nodes.IfAsync.prototype](#apidoc.module.nunjucks.nodes.IfAsync.prototype)

#### <a name="apidoc.element.nunjucks.nodes.IfAsync.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.IfAsync.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.IfAsync.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Import"></a>[module nunjucks.nodes.Import](#apidoc.module.nunjucks.nodes.Import)

#### <a name="apidoc.element.nunjucks.nodes.Import.Import"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Import ()](#apidoc.element.nunjucks.nodes.Import.Import)
- description and source-code
```javascript
Import = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	                            importTok.colno);
	        }

	        var target = this.parseExpression();

	        var withContext = this.parseWithContext();

	        var node = new nodes.Import(importTok.lineno,
	                                    importTok.colno,
	                                    template,
	                                    target,
	                                    withContext);

	        this.advanceAfterBlockEnd(importTok.value);
...
```

#### <a name="apidoc.element.nunjucks.nodes.Import.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Import.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Import.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Import.prototype"></a>[module nunjucks.nodes.Import.prototype](#apidoc.module.nunjucks.nodes.Import.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Import.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Import.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Import.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.In"></a>[module nunjucks.nodes.In](#apidoc.module.nunjucks.nodes.In)

#### <a name="apidoc.element.nunjucks.nodes.In.In"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>In ()](#apidoc.element.nunjucks.nodes.In.In)
- description and source-code
```javascript
In = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        var tok = this.nextToken();
	        if (!tok) { break; }
	        var invert = tok.type === lexer.TOKEN_SYMBOL && tok.value === 'not';
	        // if it wasn't 'not', put it back
	        if (!invert) { this.pushToken(tok); }
	        if (this.skipSymbol('in')) {
	          var node2 = this.parseCompare();
	          node = new nodes.In(node.lineno,
	                              node.colno,
	                              node,
	                              node2);
	          if (invert) {
	            node = new nodes.Not(node.lineno,
	                                 node.colno,
	                                 node);
...
```

#### <a name="apidoc.element.nunjucks.nodes.In.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.In.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.In.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.In.prototype"></a>[module nunjucks.nodes.In.prototype](#apidoc.module.nunjucks.nodes.In.prototype)

#### <a name="apidoc.element.nunjucks.nodes.In.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.In.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.In.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Include"></a>[module nunjucks.nodes.Include](#apidoc.module.nunjucks.nodes.Include)

#### <a name="apidoc.element.nunjucks.nodes.Include.Include"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Include ()](#apidoc.element.nunjucks.nodes.Include.Include)
- description and source-code
```javascript
Include = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	    parseInclude: function() {
	        var tagName = 'include';
	        var tag = this.peekToken();
	        if(!this.skipSymbol(tagName)) {
	            this.fail('parseInclude: expected '+ tagName);
	        }

	        var node = new nodes.Include(tag.lineno, tag.colno);
	        node.template = this.parseExpression();

	        if(this.skipSymbol('ignore') && this.skipSymbol('missing')) {
	            node.ignoreMissing = true;
	        }

	        this.advanceAfterBlockEnd(tag.value);
...
```

#### <a name="apidoc.element.nunjucks.nodes.Include.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Include.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Include.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Include.prototype"></a>[module nunjucks.nodes.Include.prototype](#apidoc.module.nunjucks.nodes.Include.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Include.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Include.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Include.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.InlineIf"></a>[module nunjucks.nodes.InlineIf](#apidoc.module.nunjucks.nodes.InlineIf)

#### <a name="apidoc.element.nunjucks.nodes.InlineIf.InlineIf"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>InlineIf ()](#apidoc.element.nunjucks.nodes.InlineIf.InlineIf)
- description and source-code
```javascript
InlineIf = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	    },

	    parseInlineIf: function() {
	        var node = this.parseOr();
	        if(this.skipSymbol('if')) {
	            var cond_node = this.parseOr();
	            var body_node = node;
	            node = new nodes.InlineIf(node.lineno, node.colno);
	            node.body = body_node;
	            node.cond = cond_node;
	            if(this.skipSymbol('else')) {
	                node.else_ = this.parseOr();
	            } else {
	                node.else_ = null;
	            }
...
```

#### <a name="apidoc.element.nunjucks.nodes.InlineIf.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.InlineIf.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.InlineIf.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.InlineIf.prototype"></a>[module nunjucks.nodes.InlineIf.prototype](#apidoc.module.nunjucks.nodes.InlineIf.prototype)

#### <a name="apidoc.element.nunjucks.nodes.InlineIf.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.InlineIf.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.InlineIf.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.KeywordArgs"></a>[module nunjucks.nodes.KeywordArgs](#apidoc.module.nunjucks.nodes.KeywordArgs)

#### <a name="apidoc.element.nunjucks.nodes.KeywordArgs.KeywordArgs"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>KeywordArgs ()](#apidoc.element.nunjucks.nodes.KeywordArgs.KeywordArgs)
- description and source-code
```javascript
KeywordArgs = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	                                          callerName,
	                                          callerArgs,
	                                          body);

	        // add the additional caller kwarg, adding kwargs if necessary
	        var args = macroCall.args.children;
	        if (!(args[args.length-1] instanceof nodes.KeywordArgs)) {
	          args.push(new nodes.KeywordArgs());
	        }
	        var kwargs = args[args.length - 1];
	        kwargs.addChild(new nodes.Pair(callTok.lineno,
	                                       callTok.colno,
	                                       callerName,
	                                       callerNode));
...
```

#### <a name="apidoc.element.nunjucks.nodes.KeywordArgs.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.KeywordArgs.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.KeywordArgs.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.KeywordArgs.prototype"></a>[module nunjucks.nodes.KeywordArgs.prototype](#apidoc.module.nunjucks.nodes.KeywordArgs.prototype)

#### <a name="apidoc.element.nunjucks.nodes.KeywordArgs.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.KeywordArgs.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.KeywordArgs.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Literal"></a>[module nunjucks.nodes.Literal](#apidoc.module.nunjucks.nodes.Literal)

#### <a name="apidoc.element.nunjucks.nodes.Literal.Literal"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Literal ()](#apidoc.element.nunjucks.nodes.Literal.Literal)
- description and source-code
```javascript
Literal = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	    },

	    compilePair: function(node, frame) {
	        var key = node.key;
	        var val = node.value;

	        if(key instanceof nodes.Symbol) {
	            key = new nodes.Literal(key.lineno, key.colno, key.value);
	        }
	        else if(!(key instanceof nodes.Literal &&
	                  typeof key.value === 'string')) {
	            this.fail('compilePair: Dict keys must be strings or names',
	                      key.lineno,
	                      key.colno);
	        }
...
```

#### <a name="apidoc.element.nunjucks.nodes.Literal.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Literal.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Literal.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Literal.prototype"></a>[module nunjucks.nodes.Literal.prototype](#apidoc.module.nunjucks.nodes.Literal.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Literal.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Literal.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Literal.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.LookupVal"></a>[module nunjucks.nodes.LookupVal](#apidoc.module.nunjucks.nodes.LookupVal)

#### <a name="apidoc.element.nunjucks.nodes.LookupVal.LookupVal"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>LookupVal ()](#apidoc.element.nunjucks.nodes.LookupVal.LookupVal)
- description and source-code
```javascript
LookupVal = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	            else if(tok.type === lexer.TOKEN_LEFT_BRACKET) {
	                // Reference
	                lookup = this.parseAggregate();
	                if(lookup.children.length > 1) {
	                    this.fail('invalid index');
	                }

	                node =  new nodes.LookupVal(tok.lineno,
	                                            tok.colno,
	                                            node,
	                                            lookup.children[0]);
	            }
	            else if(tok.type === lexer.TOKEN_OPERATOR && tok.value === '.') {
	                // Reference
	                this.nextToken();
...
```

#### <a name="apidoc.element.nunjucks.nodes.LookupVal.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.LookupVal.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.LookupVal.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.LookupVal.prototype"></a>[module nunjucks.nodes.LookupVal.prototype](#apidoc.module.nunjucks.nodes.LookupVal.prototype)

#### <a name="apidoc.element.nunjucks.nodes.LookupVal.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.LookupVal.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.LookupVal.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Macro"></a>[module nunjucks.nodes.Macro](#apidoc.module.nunjucks.nodes.Macro)

#### <a name="apidoc.element.nunjucks.nodes.Macro.Macro"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Macro ()](#apidoc.element.nunjucks.nodes.Macro.Macro)
- description and source-code
```javascript
Macro = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        var macroTok = this.peekToken();
	        if(!this.skipSymbol('macro')) {
	            this.fail('expected macro');
	        }

	        var name = this.parsePrimary(true);
	        var args = this.parseSignature();
	        var node = new nodes.Macro(macroTok.lineno,
	                                   macroTok.colno,
	                                   name,
	                                   args);

	        this.advanceAfterBlockEnd(macroTok.value);
	        node.body = this.parseUntilBlocks('endmacro');
	        this.advanceAfterBlockEnd();
...
```

#### <a name="apidoc.element.nunjucks.nodes.Macro.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Macro.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Macro.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Macro.prototype"></a>[module nunjucks.nodes.Macro.prototype](#apidoc.module.nunjucks.nodes.Macro.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Macro.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Macro.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Macro.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Mod"></a>[module nunjucks.nodes.Mod](#apidoc.module.nunjucks.nodes.Mod)

#### <a name="apidoc.element.nunjucks.nodes.Mod.Mod"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Mod ()](#apidoc.element.nunjucks.nodes.Mod.Mod)
- description and source-code
```javascript
Mod = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parseMod: function() {
	        var node = this.parsePow();
	        while(this.skipValue(lexer.TOKEN_OPERATOR, '%')) {
	            var node2 = this.parsePow();
	            node = new nodes.Mod(node.lineno,
	                                 node.colno,
	                                 node,
	                                 node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.Mod.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Mod.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Mod.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Mod.prototype"></a>[module nunjucks.nodes.Mod.prototype](#apidoc.module.nunjucks.nodes.Mod.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Mod.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Mod.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Mod.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Mul"></a>[module nunjucks.nodes.Mul](#apidoc.module.nunjucks.nodes.Mul)

#### <a name="apidoc.element.nunjucks.nodes.Mul.Mul"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Mul ()](#apidoc.element.nunjucks.nodes.Mul.Mul)
- description and source-code
```javascript
Mul = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parseMul: function() {
	        var node = this.parseDiv();
	        while(this.skipValue(lexer.TOKEN_OPERATOR, '*')) {
	            var node2 = this.parseDiv();
	            node = new nodes.Mul(node.lineno,
	                                 node.colno,
	                                 node,
	                                 node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.Mul.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Mul.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Mul.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Mul.prototype"></a>[module nunjucks.nodes.Mul.prototype](#apidoc.module.nunjucks.nodes.Mul.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Mul.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Mul.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Mul.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Neg"></a>[module nunjucks.nodes.Neg](#apidoc.module.nunjucks.nodes.Neg)

#### <a name="apidoc.element.nunjucks.nodes.Neg.Neg"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Neg ()](#apidoc.element.nunjucks.nodes.Neg.Neg)
- description and source-code
```javascript
Neg = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	    },

	    parseUnary: function(noFilters) {
	        var tok = this.peekToken();
	        var node;

	        if(this.skipValue(lexer.TOKEN_OPERATOR, '-')) {
	            node = new nodes.Neg(tok.lineno,
	                                 tok.colno,
	                                 this.parseUnary(true));
	        }
	        else if(this.skipValue(lexer.TOKEN_OPERATOR, '+')) {
	            node = new nodes.Pos(tok.lineno,
	                                 tok.colno,
	                                 this.parseUnary(true));
...
```

#### <a name="apidoc.element.nunjucks.nodes.Neg.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Neg.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Neg.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Neg.prototype"></a>[module nunjucks.nodes.Neg.prototype](#apidoc.module.nunjucks.nodes.Neg.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Neg.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Neg.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Neg.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Node"></a>[module nunjucks.nodes.Node](#apidoc.module.nunjucks.nodes.Node)

#### <a name="apidoc.element.nunjucks.nodes.Node.Node"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Node ()](#apidoc.element.nunjucks.nodes.Node.Node)
- description and source-code
```javascript
Node = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Node.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Node.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Node.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Node.prototype"></a>[module nunjucks.nodes.Node.prototype](#apidoc.module.nunjucks.nodes.Node.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Node.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Node.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Node.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Node.prototype.findAll"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Node.prototype.</span>findAll (type, results)](#apidoc.element.nunjucks.nodes.Node.prototype.findAll)
- description and source-code
```javascript
findAll = function (type, results) {
    results = results || [];

    var i, l;
    if(this instanceof NodeList) {
        var children = this.children;

        for(i = 0, l = children.length; i < l; i++) {
            traverseAndCheck(children[i], type, results);
        }
    }
    else {
        var fields = this.fields;

        for(i = 0, l = fields.length; i < l; i++) {
            traverseAndCheck(this[fields[i]], type, results);
        }
    }

    return results;
}
```
- example usage
```shell
...
	        this.emitLine('}');
	        this.emitFuncEnd(true);

	        this.inBlock = true;

	        var blockNames = [];

	        var i, name, block, blocks = node.findAll(nodes.Block);
	        for (i = 0; i < blocks.length; i++) {
	            block = blocks[i];
	            name = block.name.value;

	            if (blockNames.indexOf(name) !== -1) {
	                throw new Error('Block "' + name + '" defined more than once.');
	            }
...
```

#### <a name="apidoc.element.nunjucks.nodes.Node.prototype.init"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Node.prototype.</span>init (lineno, colno)](#apidoc.element.nunjucks.nodes.Node.prototype.init)
- description and source-code
```javascript
init = function (lineno, colno) {
    this.lineno = lineno;
    this.colno = colno;

    var fields = this.fields;
    for(var i = 0, l = fields.length; i < l; i++) {
        var field = fields[i];

        // The first two args are line/col numbers, so offset by 2
        var val = arguments[i + 2];

        // Fields should never be undefined, but null. It makes
        // testing easier to normalize values.
        if(val === undefined) {
            val = null;
        }

        this[field] = val;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Node.prototype.iterFields"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Node.prototype.</span>iterFields (func)](#apidoc.element.nunjucks.nodes.Node.prototype.iterFields)
- description and source-code
```javascript
iterFields = function (func) {
    lib.each(this.fields, function(field) {
        func(this[field], field);
    }, this);
}
```
- example usage
```shell
...
	            });
	        }
	    }
	    else {
	        var nodes = null;
	        var props = null;

	        node.iterFields(function(val, field) {
	            if(val instanceof Node) {
	                nodes = nodes || {};
	                nodes[field] = val;
	            }
	            else {
	                props = props || {};
	                props[field] = val;
...
```



# <a name="apidoc.module.nunjucks.nodes.NodeList"></a>[module nunjucks.nodes.NodeList](#apidoc.module.nunjucks.nodes.NodeList)

#### <a name="apidoc.element.nunjucks.nodes.NodeList.NodeList"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>NodeList ()](#apidoc.element.nunjucks.nodes.NodeList.NodeList)
- description and source-code
```javascript
NodeList = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        // a call block is parsed as a normal FunCall, but with an added
	        // 'caller' kwarg which is a Caller node.
	        var callTok = this.peekToken();
	        if(!this.skipSymbol('call')) {
	            this.fail('expected call');
	        }

	        var callerArgs = this.parseSignature(true) || new nodes.NodeList();
	        var macroCall = this.parsePrimary();

	        this.advanceAfterBlockEnd(callTok.value);
	        var body = this.parseUntilBlocks('endcall');
	        this.advanceAfterBlockEnd();

	        var callerName = new nodes.Symbol(callTok.lineno,
...
```

#### <a name="apidoc.element.nunjucks.nodes.NodeList.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.NodeList.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.NodeList.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.NodeList.prototype"></a>[module nunjucks.nodes.NodeList.prototype](#apidoc.module.nunjucks.nodes.NodeList.prototype)

#### <a name="apidoc.element.nunjucks.nodes.NodeList.prototype.addChild"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.NodeList.prototype.</span>addChild (node)](#apidoc.element.nunjucks.nodes.NodeList.prototype.addChild)
- description and source-code
```javascript
addChild = function (node) {
    this.children.push(node);
}
```
- example usage
```shell
...
	        }

	        var type = this.peekToken().type;
	        if(type === lexer.TOKEN_COMMA) {
	            // key/value iteration
	            var key = node.name;
	            node.name = new nodes.Array(key.lineno, key.colno);
	            node.name.addChild(key);

	            while(this.skip(lexer.TOKEN_COMMA)) {
	                var prim = this.parsePrimary();
	                node.name.addChild(prim);
	            }
	        }
...
```

#### <a name="apidoc.element.nunjucks.nodes.NodeList.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.NodeList.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.NodeList.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.NodeList.prototype.init"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.NodeList.prototype.</span>init ()](#apidoc.element.nunjucks.nodes.NodeList.prototype.init)
- description and source-code
```javascript
init = function () {
    // Save the current parent method
    var tmp = this.parent;

    // Set parent to the previous method, call, and restore
    this.parent = parent;
    var res = src.apply(this, arguments);
    this.parent = tmp;

    return res;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Not"></a>[module nunjucks.nodes.Not](#apidoc.module.nunjucks.nodes.Not)

#### <a name="apidoc.element.nunjucks.nodes.Not.Not"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Not ()](#apidoc.element.nunjucks.nodes.Not.Not)
- description and source-code
```javascript
Not = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        }
	        return node;
	    },

	    parseNot: function() {
	        var tok = this.peekToken();
	        if(this.skipSymbol('not')) {
	            return new nodes.Not(tok.lineno,
	                                 tok.colno,
	                                 this.parseNot());
	        }
	        return this.parseIn();
	    },

	    parseIn: function() {
...
```

#### <a name="apidoc.element.nunjucks.nodes.Not.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Not.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Not.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Not.prototype"></a>[module nunjucks.nodes.Not.prototype](#apidoc.module.nunjucks.nodes.Not.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Not.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Not.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Not.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Or"></a>[module nunjucks.nodes.Or](#apidoc.module.nunjucks.nodes.Or)

#### <a name="apidoc.element.nunjucks.nodes.Or.Or"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Or ()](#apidoc.element.nunjucks.nodes.Or.Or)
- description and source-code
```javascript
Or = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parseOr: function() {
	        var node = this.parseAnd();
	        while(this.skipSymbol('or')) {
	            var node2 = this.parseAnd();
	            node = new nodes.Or(node.lineno,
	                                node.colno,
	                                node,
	                                node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.Or.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Or.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Or.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Or.prototype"></a>[module nunjucks.nodes.Or.prototype](#apidoc.module.nunjucks.nodes.Or.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Or.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Or.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Or.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Output"></a>[module nunjucks.nodes.Output](#apidoc.module.nunjucks.nodes.Output)

#### <a name="apidoc.element.nunjucks.nodes.Output.Output"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Output ()](#apidoc.element.nunjucks.nodes.Output.Output)
- description and source-code
```javascript
Output = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        }
	        var kwargs = args[args.length - 1];
	        kwargs.addChild(new nodes.Pair(callTok.lineno,
	                                       callTok.colno,
	                                       callerName,
	                                       callerNode));

	        return new nodes.Output(callTok.lineno,
	                                callTok.colno,
	                                [macroCall]);
	    },

	    parseWithContext: function() {
	        var tok = this.peekToken();
...
```

#### <a name="apidoc.element.nunjucks.nodes.Output.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Output.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Output.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Output.prototype"></a>[module nunjucks.nodes.Output.prototype](#apidoc.module.nunjucks.nodes.Output.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Output.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Output.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Output.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Pair"></a>[module nunjucks.nodes.Pair](#apidoc.module.nunjucks.nodes.Pair)

#### <a name="apidoc.element.nunjucks.nodes.Pair.Pair"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Pair ()](#apidoc.element.nunjucks.nodes.Pair.Pair)
- description and source-code
```javascript
Pair = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...

	        // add the additional caller kwarg, adding kwargs if necessary
	        var args = macroCall.args.children;
	        if (!(args[args.length-1] instanceof nodes.KeywordArgs)) {
	          args.push(new nodes.KeywordArgs());
	        }
	        var kwargs = args[args.length - 1];
	        kwargs.addChild(new nodes.Pair(callTok.lineno,
	                                       callTok.colno,
	                                       callerName,
	                                       callerNode));

	        return new nodes.Output(callTok.lineno,
	                                callTok.colno,
	                                [macroCall]);
...
```

#### <a name="apidoc.element.nunjucks.nodes.Pair.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Pair.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Pair.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Pair.prototype"></a>[module nunjucks.nodes.Pair.prototype](#apidoc.module.nunjucks.nodes.Pair.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Pair.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Pair.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Pair.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Pos"></a>[module nunjucks.nodes.Pos](#apidoc.module.nunjucks.nodes.Pos)

#### <a name="apidoc.element.nunjucks.nodes.Pos.Pos"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Pos ()](#apidoc.element.nunjucks.nodes.Pos.Pos)
- description and source-code
```javascript
Pos = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...

	        if(this.skipValue(lexer.TOKEN_OPERATOR, '-')) {
	            node = new nodes.Neg(tok.lineno,
	                                 tok.colno,
	                                 this.parseUnary(true));
	        }
	        else if(this.skipValue(lexer.TOKEN_OPERATOR, '+')) {
	            node = new nodes.Pos(tok.lineno,
	                                 tok.colno,
	                                 this.parseUnary(true));
	        }
	        else {
	            node = this.parsePrimary();
	        }
...
```

#### <a name="apidoc.element.nunjucks.nodes.Pos.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Pos.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Pos.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Pos.prototype"></a>[module nunjucks.nodes.Pos.prototype](#apidoc.module.nunjucks.nodes.Pos.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Pos.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Pos.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Pos.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Pow"></a>[module nunjucks.nodes.Pow](#apidoc.module.nunjucks.nodes.Pow)

#### <a name="apidoc.element.nunjucks.nodes.Pow.Pow"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Pow ()](#apidoc.element.nunjucks.nodes.Pow.Pow)
- description and source-code
```javascript
Pow = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parsePow: function() {
	        var node = this.parseUnary();
	        while(this.skipValue(lexer.TOKEN_OPERATOR, '**')) {
	            var node2 = this.parseUnary();
	            node = new nodes.Pow(node.lineno,
	                                 node.colno,
	                                 node,
	                                 node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.Pow.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Pow.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Pow.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Pow.prototype"></a>[module nunjucks.nodes.Pow.prototype](#apidoc.module.nunjucks.nodes.Pow.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Pow.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Pow.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Pow.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Root"></a>[module nunjucks.nodes.Root](#apidoc.module.nunjucks.nodes.Root)

#### <a name="apidoc.element.nunjucks.nodes.Root.Root"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Root ()](#apidoc.element.nunjucks.nodes.Root.Root)
- description and source-code
```javascript
Root = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	    },

	    parse: function() {
	        return new nodes.NodeList(0, 0, this.parseNodes());
	    },

	    parseAsRoot: function() {
	        return new nodes.Root(0, 0, this.parseNodes());
	    }
	});

	// var util = require('util');

	// var l = lexer.lex('{%- if x -%}\n hello {% endif %}');
	// var t;
...
```

#### <a name="apidoc.element.nunjucks.nodes.Root.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Root.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Root.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Root.prototype"></a>[module nunjucks.nodes.Root.prototype](#apidoc.module.nunjucks.nodes.Root.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Root.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Root.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Root.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Set"></a>[module nunjucks.nodes.Set](#apidoc.module.nunjucks.nodes.Set)

#### <a name="apidoc.element.nunjucks.nodes.Set.Set"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Set ()](#apidoc.element.nunjucks.nodes.Set.Set)
- description and source-code
```javascript
Set = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...

	    parseSet: function() {
	        var tag = this.peekToken();
	        if(!this.skipSymbol('set')) {
	            this.fail('parseSet: expected set', tag.lineno, tag.colno);
	        }

	        var node = new nodes.Set(tag.lineno, tag.colno, []);

	        var target;
	        while((target = this.parsePrimary())) {
	            node.targets.push(target);

	            if(!this.skip(lexer.TOKEN_COMMA)) {
	                break;
...
```

#### <a name="apidoc.element.nunjucks.nodes.Set.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Set.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Set.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Set.prototype"></a>[module nunjucks.nodes.Set.prototype](#apidoc.module.nunjucks.nodes.Set.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Set.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Set.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Set.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Sub"></a>[module nunjucks.nodes.Sub](#apidoc.module.nunjucks.nodes.Sub)

#### <a name="apidoc.element.nunjucks.nodes.Sub.Sub"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Sub ()](#apidoc.element.nunjucks.nodes.Sub.Sub)
- description and source-code
```javascript
Sub = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        return node;
	    },

	    parseSub: function() {
	        var node = this.parseMul();
	        while(this.skipValue(lexer.TOKEN_OPERATOR, '-')) {
	            var node2 = this.parseMul();
	            node = new nodes.Sub(node.lineno,
	                                 node.colno,
	                                 node,
	                                 node2);
	        }
	        return node;
	    },
...
```

#### <a name="apidoc.element.nunjucks.nodes.Sub.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Sub.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Sub.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Sub.prototype"></a>[module nunjucks.nodes.Sub.prototype](#apidoc.module.nunjucks.nodes.Sub.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Sub.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Sub.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Sub.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Super"></a>[module nunjucks.nodes.Super](#apidoc.module.nunjucks.nodes.Super)

#### <a name="apidoc.element.nunjucks.nodes.Super.Super"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Super ()](#apidoc.element.nunjucks.nodes.Super.Super)
- description and source-code
```javascript
Super = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	               node.name.value === 'super') {
	                hasSuper = true;
	                return new nodes.Symbol(node.lineno, node.colno, symbol);
	            }
	        });

	        if(hasSuper) {
	            blockNode.body.children.unshift(new nodes.Super(
	                0, 0, blockNode.name, new nodes.Symbol(0, 0, symbol)
	            ));
	        }
	    });
	}

	function convertStatements(ast) {
...
```

#### <a name="apidoc.element.nunjucks.nodes.Super.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Super.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Super.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Super.prototype"></a>[module nunjucks.nodes.Super.prototype](#apidoc.module.nunjucks.nodes.Super.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Super.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Super.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Super.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Symbol"></a>[module nunjucks.nodes.Symbol](#apidoc.module.nunjucks.nodes.Symbol)

#### <a name="apidoc.element.nunjucks.nodes.Symbol.Symbol"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Symbol ()](#apidoc.element.nunjucks.nodes.Symbol.Symbol)
- description and source-code
```javascript
Symbol = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        var callerArgs = this.parseSignature(true) || new nodes.NodeList();
	        var macroCall = this.parsePrimary();

	        this.advanceAfterBlockEnd(callTok.value);
	        var body = this.parseUntilBlocks('endcall');
	        this.advanceAfterBlockEnd();

	        var callerName = new nodes.Symbol(callTok.lineno,
	                                          callTok.colno,
	                                          'caller');
	        var callerNode = new nodes.Caller(callTok.lineno,
	                                          callTok.colno,
	                                          callerName,
	                                          callerArgs,
	                                          body);
...
```

#### <a name="apidoc.element.nunjucks.nodes.Symbol.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Symbol.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Symbol.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Symbol.prototype"></a>[module nunjucks.nodes.Symbol.prototype](#apidoc.module.nunjucks.nodes.Symbol.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Symbol.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Symbol.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Symbol.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.TemplateData"></a>[module nunjucks.nodes.TemplateData](#apidoc.module.nunjucks.nodes.TemplateData)

#### <a name="apidoc.element.nunjucks.nodes.TemplateData.TemplateData"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>TemplateData ()](#apidoc.element.nunjucks.nodes.TemplateData.TemplateData)
- description and source-code
```javascript
TemplateData = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	                str += all;
	            }
	        }

	        return new nodes.Output(
	            begun.lineno,
	            begun.colno,
	            [new nodes.TemplateData(begun.lineno, begun.colno, str)]
	        );
	    },

	    parsePostfix: function(node) {
	        var lookup, tok = this.peekToken();

	        while(tok) {
...
```

#### <a name="apidoc.element.nunjucks.nodes.TemplateData.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.TemplateData.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.TemplateData.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.TemplateData.prototype"></a>[module nunjucks.nodes.TemplateData.prototype](#apidoc.module.nunjucks.nodes.TemplateData.prototype)

#### <a name="apidoc.element.nunjucks.nodes.TemplateData.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.TemplateData.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.TemplateData.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nodes.Value"></a>[module nunjucks.nodes.Value](#apidoc.module.nunjucks.nodes.Value)

#### <a name="apidoc.element.nunjucks.nodes.Value.Value"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.</span>Value ()](#apidoc.element.nunjucks.nodes.Value.Value)
- description and source-code
```javascript
Value = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nodes.Value.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Value.</span>extend (name, props)](#apidoc.element.nunjucks.nodes.Value.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.nodes.Value.prototype"></a>[module nunjucks.nodes.Value.prototype](#apidoc.module.nunjucks.nodes.Value.prototype)

#### <a name="apidoc.element.nunjucks.nodes.Value.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.nodes.Value.prototype.</span>constructor ()](#apidoc.element.nunjucks.nodes.Value.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.nunjucks"></a>[module nunjucks.nunjucks](#apidoc.module.nunjucks.nunjucks)

#### <a name="apidoc.element.nunjucks.nunjucks.Environment"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>Environment ()](#apidoc.element.nunjucks.nunjucks.Environment)
- description and source-code
```javascript
Environment = function () {
	        if(prototype.init) {
	            prototype.init.apply(this, arguments);
	        }
	    }
```
- example usage
```shell
...
    else if(loaders.WebLoader) {
        TemplateLoader = new loaders.WebLoader(templatesPath, {
            useCache: opts.web && opts.web.useCache,
            async: opts.web && opts.web.async
        });
    }

    e = new env.Environment(TemplateLoader, opts);

    if(opts && opts.express) {
        e.express(opts.express);
    }

    return e;
};
...
```

#### <a name="apidoc.element.nunjucks.nunjucks.Loader"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>Loader ()](#apidoc.element.nunjucks.nunjucks.Loader)
- description and source-code
```javascript
Loader = function () {
	        if(prototype.init) {
	            prototype.init.apply(this, arguments);
	        }
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nunjucks.PrecompiledLoader"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>PrecompiledLoader ()](#apidoc.element.nunjucks.nunjucks.PrecompiledLoader)
- description and source-code
```javascript
PrecompiledLoader = function () {
	        if(prototype.init) {
	            prototype.init.apply(this, arguments);
	        }
	    }
```
- example usage
```shell
...
	        }

	        // It's easy to use precompiled templates: just include them
	        // before you configure nunjucks and this will automatically
	        // pick it up and use it
	        if((true) && window.nunjucksPrecompiled) {
	            this.loaders.unshift(
	                new builtin_loaders.PrecompiledLoader(window.nunjucksPrecompiled)
	            );
	        }

	        this.initCache();

	        this.globals = globals();
	        this.filters = {};
...
```

#### <a name="apidoc.element.nunjucks.nunjucks.Template"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>Template ()](#apidoc.element.nunjucks.nunjucks.Template)
- description and source-code
```javascript
Template = function () {
	        if(prototype.init) {
	            prototype.init.apply(this, arguments);
	        }
	    }
```
- example usage
```shell
...
return e;
};

module.exports.compile = function(src, env, path, eagerCompile) {
if(!e) {
    module.exports.configure();
}
return new module.exports.Template(src, env, path, eagerCompile);
};

module.exports.render = function(name, ctx, cb) {
if(!e) {
    module.exports.configure();
}
...
```

#### <a name="apidoc.element.nunjucks.nunjucks.WebLoader"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>WebLoader ()](#apidoc.element.nunjucks.nunjucks.WebLoader)
- description and source-code
```javascript
WebLoader = function () {
	        if(prototype.init) {
	            prototype.init.apply(this, arguments);
	        }
	    }
```
- example usage
```shell
...
if(loaders.FileSystemLoader) {
    TemplateLoader = new loaders.FileSystemLoader(templatesPath, {
        watch: opts.watch,
        noCache: opts.noCache
    });
}
else if(loaders.WebLoader) {
    TemplateLoader = new loaders.WebLoader(templatesPath, {
        useCache: opts.web && opts.web.useCache,
        async: opts.web && opts.web.async
    });
}

e = new env.Environment(TemplateLoader, opts);
...
```

#### <a name="apidoc.element.nunjucks.nunjucks.compile"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>compile (src, env, path, eagerCompile)](#apidoc.element.nunjucks.nunjucks.compile)
- description and source-code
```javascript
compile = function (src, env, path, eagerCompile) {
	    if(!e) {
	        module.exports.configure();
	    }
	    return new module.exports.Template(src, env, path, eagerCompile);
	}
```
- example usage
```shell
...
	                tmpl = this.loaders[i].cache[_name];
	                if (tmpl) break;
	            }
	        }

	        if(tmpl) {
	            if(eagerCompile) {
	                tmpl.compile();
	            }

	            if(cb) {
	                cb(null, tmpl);
	            }
	            else {
	                return tmpl;
...
```

#### <a name="apidoc.element.nunjucks.nunjucks.configure"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>configure (templatesPath, opts)](#apidoc.element.nunjucks.nunjucks.configure)
- description and source-code
```javascript
configure = function (templatesPath, opts) {
	    opts = opts || {};
	    if(lib.isObject(templatesPath)) {
	        opts = templatesPath;
	        templatesPath = null;
	    }

	    var TemplateLoader;
	    if(loaders.FileSystemLoader) {
	        TemplateLoader = new loaders.FileSystemLoader(templatesPath, {
	            watch: opts.watch,
	            noCache: opts.noCache
	        });
	    }
	    else if(loaders.WebLoader) {
	        TemplateLoader = new loaders.WebLoader(templatesPath, {
	            useCache: opts.web && opts.web.useCache,
	            async: opts.web && opts.web.async
	        });
	    }

	    e = new env.Environment(TemplateLoader, opts);

	    if(opts && opts.express) {
	        e.express(opts.express);
	    }

	    return e;
	}
```
- example usage
```shell
...
}

return e;
};

module.exports.compile = function(src, env, path, eagerCompile) {
if(!e) {
    module.exports.configure();
}
return new module.exports.Template(src, env, path, eagerCompile);
};

module.exports.render = function(name, ctx, cb) {
if(!e) {
    module.exports.configure();
...
```

#### <a name="apidoc.element.nunjucks.nunjucks.installJinjaCompat"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>installJinjaCompat ()](#apidoc.element.nunjucks.nunjucks.installJinjaCompat)
- description and source-code
```javascript
function installCompat() {
	  'use strict';

	  // This must be called like 'nunjucks.installCompat' so that 'this'
	  // references the nunjucks instance
	  var runtime = this.runtime; // jshint ignore:line
	  var lib = this.lib; // jshint ignore:line

	  var orig_contextOrFrameLookup = runtime.contextOrFrameLookup;
	  runtime.contextOrFrameLookup = function(context, frame, key) {
	    var val = orig_contextOrFrameLookup.apply(this, arguments);
	    if (val === undefined) {
	      switch (key) {
	      case 'True':
	        return true;
	      case 'False':
	        return false;
	      case 'None':
	        return null;
	      }
	    }

	    return val;
	  };

	  var orig_memberLookup = runtime.memberLookup;
	  var ARRAY_MEMBERS = {
	    pop: function(index) {
	      if (index === undefined) {
	        return this.pop();
	      }
	      if (index >= this.length || index < 0) {
	        throw new Error('KeyError');
	      }
	      return this.splice(index, 1);
	    },
	    append: function(element) {
	        return this.push(element);
	    },
	    remove: function(element) {
	      for (var i = 0; i < this.length; i++) {
	        if (this[i] === element) {
	          return this.splice(i, 1);
	        }
	      }
	      throw new Error('ValueError');
	    },
	    count: function(element) {
	      var count = 0;
	      for (var i = 0; i < this.length; i++) {
	        if (this[i] === element) {
	          count++;
	        }
	      }
	      return count;
	    },
	    index: function(element) {
	      var i;
	      if ((i = this.indexOf(element)) === -1) {
	        throw new Error('ValueError');
	      }
	      return i;
	    },
	    find: function(element) {
	      return this.indexOf(element);
	    },
	    insert: function(index, elem) {
	      return this.splice(index, 0, elem);
	    }
	  };
	  var OBJECT_MEMBERS = {
	    items: function() {
	      var ret = [];
	      for(var k in this) {
	        ret.push([k, this[k]]);
	      }
	      return ret;
	    },
	    values: function() {
	      var ret = [];
	      for(var k in this) {
	        ret.push(this[k]);
	      }
	      return ret;
	    },
	    keys: function() {
	      var ret = [];
	      for(var k in this) {
	        ret.push(k);
	      }
	      return ret;
	    },
	    get: function(key, def) {
	      var output = this[key];
	      if (output === undefined) {
	        output = def;
	      }
	      return output;
	    },
	    has_key: function(key) {
	      return this.hasOwnProperty(key);
	    },
	    pop: function(key, def) {
	      var output = this[key];
	      if (output === undefined && def !== undefined) {
	        output = def;
	      } else if (output === undefined) {
	        throw new Error('KeyError');
	      } else {
	        delete this[key];
	      }
	      return output;
	    },
	    popitem: function() {
	      for (var k in this) {
	        // Return the first object pair.
	        var val = this[k];
	        delete this[k];
	        return [k, val];
	      }
	      throw new Error('KeyError');
	    },
	    setdefault: function(key, def) {
	      if (key in this) {
	        return this[key];
	      }
	      if (def === undefined) {
	        def = null;
	      }
	      return this[key] = def;
	    },
	    update: function(kwargs) {
	      for (var k in kwargs) {
	        this[k] = kwargs[k];
	      }
	      return null;  // Always returns None
	    }
	  };
	  OBJECT_MEMBERS.iteritems = OBJECT_MEMBERS.items;
	  OBJECT_MEMBERS.itervalues = OBJECT_MEMBERS.values;
	  OBJECT_MEMBERS.iterkeys = OBJECT_MEMBERS.keys;
	  runtime.memberLookup = function(obj, val, autoescape) { // jshint ignore:line
	    obj = obj || {};

	    // If the object is an object, return any of the methods that Python would
	    // otherwise provide.
	    if (lib.isArray(obj) && ARRAY_MEMBERS.hasOwnProperty(val)) {
	      return function() {return ARRAY_MEMBERS[val].apply(obj, arguments);};
	    }

	    if (lib.isObject(obj) && OBJECT_MEMBERS.hasOwnProperty(val)) {
	      return function() {return OBJECT_MEMBERS[val].apply(obj, arguments);};
	    }

	    return orig_memberLookup.a ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nunjucks.render"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>render (name, ctx, cb)](#apidoc.element.nunjucks.nunjucks.render)
- description and source-code
```javascript
render = function (name, ctx, cb) {
	    if(!e) {
	        module.exports.configure();
	    }

	    return e.render(name, ctx, cb);
	}
```
- example usage
```shell
...
};

module.exports.render = function(name, ctx, cb) {
if(!e) {
    module.exports.configure();
}

return e.render(name, ctx, cb);
};

module.exports.renderString = function(src, ctx, cb) {
if(!e) {
    module.exports.configure();
}
...
```

#### <a name="apidoc.element.nunjucks.nunjucks.renderString"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks.</span>renderString (src, ctx, cb)](#apidoc.element.nunjucks.nunjucks.renderString)
- description and source-code
```javascript
renderString = function (src, ctx, cb) {
	    if(!e) {
	        module.exports.configure();
	    }

	    return e.renderString(src, ctx, cb);
	}
```
- example usage
```shell
...
};

module.exports.renderString = function(src, ctx, cb) {
    if(!e) {
        module.exports.configure();
    }

    return e.renderString(src, ctx, cb);
};

if(precompile) {
    module.exports.precompile = precompile.precompile;
    module.exports.precompileString = precompile.precompileString;
}
...
```



# <a name="apidoc.module.nunjucks.nunjucks_slim"></a>[module nunjucks.nunjucks_slim](#apidoc.module.nunjucks.nunjucks_slim)

#### <a name="apidoc.element.nunjucks.nunjucks_slim.Environment"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>Environment ()](#apidoc.element.nunjucks.nunjucks_slim.Environment)
- description and source-code
```javascript
Environment = function () {
	        if(prototype.init) {
	            prototype.init.apply(this, arguments);
	        }
	    }
```
- example usage
```shell
...
    else if(loaders.WebLoader) {
        TemplateLoader = new loaders.WebLoader(templatesPath, {
            useCache: opts.web && opts.web.useCache,
            async: opts.web && opts.web.async
        });
    }

    e = new env.Environment(TemplateLoader, opts);

    if(opts && opts.express) {
        e.express(opts.express);
    }

    return e;
};
...
```

#### <a name="apidoc.element.nunjucks.nunjucks_slim.Loader"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>Loader ()](#apidoc.element.nunjucks.nunjucks_slim.Loader)
- description and source-code
```javascript
Loader = function () {
	        if(prototype.init) {
	            prototype.init.apply(this, arguments);
	        }
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nunjucks_slim.PrecompiledLoader"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>PrecompiledLoader ()](#apidoc.element.nunjucks.nunjucks_slim.PrecompiledLoader)
- description and source-code
```javascript
PrecompiledLoader = function () {
	        if(prototype.init) {
	            prototype.init.apply(this, arguments);
	        }
	    }
```
- example usage
```shell
...
	        }

	        // It's easy to use precompiled templates: just include them
	        // before you configure nunjucks and this will automatically
	        // pick it up and use it
	        if((true) && window.nunjucksPrecompiled) {
	            this.loaders.unshift(
	                new builtin_loaders.PrecompiledLoader(window.nunjucksPrecompiled)
	            );
	        }

	        this.initCache();

	        this.globals = globals();
	        this.filters = {};
...
```

#### <a name="apidoc.element.nunjucks.nunjucks_slim.Template"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>Template ()](#apidoc.element.nunjucks.nunjucks_slim.Template)
- description and source-code
```javascript
Template = function () {
	        if(prototype.init) {
	            prototype.init.apply(this, arguments);
	        }
	    }
```
- example usage
```shell
...
return e;
};

module.exports.compile = function(src, env, path, eagerCompile) {
if(!e) {
    module.exports.configure();
}
return new module.exports.Template(src, env, path, eagerCompile);
};

module.exports.render = function(name, ctx, cb) {
if(!e) {
    module.exports.configure();
}
...
```

#### <a name="apidoc.element.nunjucks.nunjucks_slim.compile"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>compile (src, env, path, eagerCompile)](#apidoc.element.nunjucks.nunjucks_slim.compile)
- description and source-code
```javascript
compile = function (src, env, path, eagerCompile) {
	    if(!e) {
	        module.exports.configure();
	    }
	    return new module.exports.Template(src, env, path, eagerCompile);
	}
```
- example usage
```shell
...
	                tmpl = this.loaders[i].cache[_name];
	                if (tmpl) break;
	            }
	        }

	        if(tmpl) {
	            if(eagerCompile) {
	                tmpl.compile();
	            }

	            if(cb) {
	                cb(null, tmpl);
	            }
	            else {
	                return tmpl;
...
```

#### <a name="apidoc.element.nunjucks.nunjucks_slim.configure"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>configure (templatesPath, opts)](#apidoc.element.nunjucks.nunjucks_slim.configure)
- description and source-code
```javascript
configure = function (templatesPath, opts) {
	    opts = opts || {};
	    if(lib.isObject(templatesPath)) {
	        opts = templatesPath;
	        templatesPath = null;
	    }

	    var TemplateLoader;
	    if(loaders.FileSystemLoader) {
	        TemplateLoader = new loaders.FileSystemLoader(templatesPath, {
	            watch: opts.watch,
	            noCache: opts.noCache
	        });
	    }
	    else if(loaders.WebLoader) {
	        TemplateLoader = new loaders.WebLoader(templatesPath, {
	            useCache: opts.web && opts.web.useCache,
	            async: opts.web && opts.web.async
	        });
	    }

	    e = new env.Environment(TemplateLoader, opts);

	    if(opts && opts.express) {
	        e.express(opts.express);
	    }

	    return e;
	}
```
- example usage
```shell
...
}

return e;
};

module.exports.compile = function(src, env, path, eagerCompile) {
if(!e) {
    module.exports.configure();
}
return new module.exports.Template(src, env, path, eagerCompile);
};

module.exports.render = function(name, ctx, cb) {
if(!e) {
    module.exports.configure();
...
```

#### <a name="apidoc.element.nunjucks.nunjucks_slim.installJinjaCompat"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>installJinjaCompat ()](#apidoc.element.nunjucks.nunjucks_slim.installJinjaCompat)
- description and source-code
```javascript
function installCompat() {
	  'use strict';

	  // This must be called like 'nunjucks.installCompat' so that 'this'
	  // references the nunjucks instance
	  var runtime = this.runtime; // jshint ignore:line
	  var lib = this.lib; // jshint ignore:line

	  var orig_contextOrFrameLookup = runtime.contextOrFrameLookup;
	  runtime.contextOrFrameLookup = function(context, frame, key) {
	    var val = orig_contextOrFrameLookup.apply(this, arguments);
	    if (val === undefined) {
	      switch (key) {
	      case 'True':
	        return true;
	      case 'False':
	        return false;
	      case 'None':
	        return null;
	      }
	    }

	    return val;
	  };

	  var orig_memberLookup = runtime.memberLookup;
	  var ARRAY_MEMBERS = {
	    pop: function(index) {
	      if (index === undefined) {
	        return this.pop();
	      }
	      if (index >= this.length || index < 0) {
	        throw new Error('KeyError');
	      }
	      return this.splice(index, 1);
	    },
	    append: function(element) {
	        return this.push(element);
	    },
	    remove: function(element) {
	      for (var i = 0; i < this.length; i++) {
	        if (this[i] === element) {
	          return this.splice(i, 1);
	        }
	      }
	      throw new Error('ValueError');
	    },
	    count: function(element) {
	      var count = 0;
	      for (var i = 0; i < this.length; i++) {
	        if (this[i] === element) {
	          count++;
	        }
	      }
	      return count;
	    },
	    index: function(element) {
	      var i;
	      if ((i = this.indexOf(element)) === -1) {
	        throw new Error('ValueError');
	      }
	      return i;
	    },
	    find: function(element) {
	      return this.indexOf(element);
	    },
	    insert: function(index, elem) {
	      return this.splice(index, 0, elem);
	    }
	  };
	  var OBJECT_MEMBERS = {
	    items: function() {
	      var ret = [];
	      for(var k in this) {
	        ret.push([k, this[k]]);
	      }
	      return ret;
	    },
	    values: function() {
	      var ret = [];
	      for(var k in this) {
	        ret.push(this[k]);
	      }
	      return ret;
	    },
	    keys: function() {
	      var ret = [];
	      for(var k in this) {
	        ret.push(k);
	      }
	      return ret;
	    },
	    get: function(key, def) {
	      var output = this[key];
	      if (output === undefined) {
	        output = def;
	      }
	      return output;
	    },
	    has_key: function(key) {
	      return this.hasOwnProperty(key);
	    },
	    pop: function(key, def) {
	      var output = this[key];
	      if (output === undefined && def !== undefined) {
	        output = def;
	      } else if (output === undefined) {
	        throw new Error('KeyError');
	      } else {
	        delete this[key];
	      }
	      return output;
	    },
	    popitem: function() {
	      for (var k in this) {
	        // Return the first object pair.
	        var val = this[k];
	        delete this[k];
	        return [k, val];
	      }
	      throw new Error('KeyError');
	    },
	    setdefault: function(key, def) {
	      if (key in this) {
	        return this[key];
	      }
	      if (def === undefined) {
	        def = null;
	      }
	      return this[key] = def;
	    },
	    update: function(kwargs) {
	      for (var k in kwargs) {
	        this[k] = kwargs[k];
	      }
	      return null;  // Always returns None
	    }
	  };
	  OBJECT_MEMBERS.iteritems = OBJECT_MEMBERS.items;
	  OBJECT_MEMBERS.itervalues = OBJECT_MEMBERS.values;
	  OBJECT_MEMBERS.iterkeys = OBJECT_MEMBERS.keys;
	  runtime.memberLookup = function(obj, val, autoescape) { // jshint ignore:line
	    obj = obj || {};

	    // If the object is an object, return any of the methods that Python would
	    // otherwise provide.
	    if (lib.isArray(obj) && ARRAY_MEMBERS.hasOwnProperty(val)) {
	      return function() {return ARRAY_MEMBERS[val].apply(obj, arguments);};
	    }

	    if (lib.isObject(obj) && OBJECT_MEMBERS.hasOwnProperty(val)) {
	      return function() {return OBJECT_MEMBERS[val].apply(obj, arguments);};
	    }

	    return orig_memberLookup.a ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.nunjucks_slim.render"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>render (name, ctx, cb)](#apidoc.element.nunjucks.nunjucks_slim.render)
- description and source-code
```javascript
render = function (name, ctx, cb) {
	    if(!e) {
	        module.exports.configure();
	    }

	    return e.render(name, ctx, cb);
	}
```
- example usage
```shell
...
};

module.exports.render = function(name, ctx, cb) {
if(!e) {
    module.exports.configure();
}

return e.render(name, ctx, cb);
};

module.exports.renderString = function(src, ctx, cb) {
if(!e) {
    module.exports.configure();
}
...
```

#### <a name="apidoc.element.nunjucks.nunjucks_slim.renderString"></a>[function <span class="apidocSignatureSpan">nunjucks.nunjucks_slim.</span>renderString (src, ctx, cb)](#apidoc.element.nunjucks.nunjucks_slim.renderString)
- description and source-code
```javascript
renderString = function (src, ctx, cb) {
	    if(!e) {
	        module.exports.configure();
	    }

	    return e.renderString(src, ctx, cb);
	}
```
- example usage
```shell
...
};

module.exports.renderString = function(src, ctx, cb) {
    if(!e) {
        module.exports.configure();
    }

    return e.renderString(src, ctx, cb);
};

if(precompile) {
    module.exports.precompile = precompile.precompile;
    module.exports.precompileString = precompile.precompileString;
}
...
```



# <a name="apidoc.module.nunjucks.object"></a>[module nunjucks.object](#apidoc.module.nunjucks.object)

#### <a name="apidoc.element.nunjucks.object.object"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>object ()](#apidoc.element.nunjucks.object.object)
- description and source-code
```javascript
object = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.object.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.object.</span>extend (name, props)](#apidoc.element.nunjucks.object.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.object.prototype"></a>[module nunjucks.object.prototype](#apidoc.module.nunjucks.object.prototype)

#### <a name="apidoc.element.nunjucks.object.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.object.prototype.</span>constructor ()](#apidoc.element.nunjucks.object.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.parser"></a>[module nunjucks.parser](#apidoc.module.nunjucks.parser)

#### <a name="apidoc.element.nunjucks.parser.parse"></a>[function <span class="apidocSignatureSpan">nunjucks.parser.</span>parse (src, extensions, opts)](#apidoc.element.nunjucks.parser.parse)
- description and source-code
```javascript
parse = function (src, extensions, opts) {
    var p = new Parser(lexer.lex(src, opts));
    if (extensions !== undefined) {
        p.extensions = extensions;
    }
    return p.parseAsRoot();
}
```
- example usage
```shell
...
	    }
	});

	// var c = new Compiler();
	// var src = 'hello {% filter title %}' +
	//     'Hello madam how are you' +
	//     '{% endfilter %}'
	// var ast = transformer.transform(parser.parse(src));
	// nodes.printNodes(ast);
	// c.compile(ast);
	// var tmpl = c.getCode();
	// console.log(tmpl);

	module.exports = {
	    compile: function(src, asyncFilters, extensions, name, opts) {
...
```



# <a name="apidoc.module.nunjucks.precompile"></a>[module nunjucks.precompile](#apidoc.module.nunjucks.precompile)

#### <a name="apidoc.element.nunjucks.precompile.precompile"></a>[function <span class="apidocSignatureSpan">nunjucks.</span>precompile (input, opts)](#apidoc.element.nunjucks.precompile.precompile)
- description and source-code
```javascript
function precompile(input, opts) {
    // The following options are available:
    //
    // * name: name of the template (auto-generated when compiling a directory)
    // * isString: input is a string, not a file path
    // * asFunction: generate a callable function
    // * force: keep compiling on error
    // * env: the Environment to use (gets extensions and async filters from it)
    // * include: which file/folders to include (folders are auto-included, files are auto-excluded)
    // * exclude: which file/folders to exclude (folders are auto-included, files are auto-excluded)
    // * wrapper: function(templates, opts) {...}
    //       Customize the output format to store the compiled template.
    //       By default, templates are stored in a global variable used by the runtime.
    //       A custom loader will be necessary to load your custom wrapper.

    opts = opts || {};
    var env = opts.env || new Environment([]);
    var wrapper = opts.wrapper || precompileGlobal;

    var pathStats = fs.existsSync(input) && fs.statSync(input);
    var precompiled = [];
    var templates = [];

    function addTemplates(dir) {
        var files = fs.readdirSync(dir);

        for(var i=0; i<files.length; i++) {
            var filepath = path.join(dir, files[i]);
            var subpath = filepath.substr(path.join(input, '/').length);
            var stat = fs.statSync(filepath);

            if(stat && stat.isDirectory()) {
                subpath += '/';
                if (!match(subpath, opts.exclude)) {
                    addTemplates(filepath);
                }
            }
            else if(match(subpath, opts.include)) {
                templates.push(filepath);
            }
        }
    }

    if(opts.isString) {
        if(!opts.name) {
            throw new Error('the "name" option is required when ' +
                            'compiling a string');
        }

        precompiled.push( _precompile(
            input,
            opts.name,
            env
        ) );
    }
    else if(pathStats.isFile()) {
        precompiled.push( _precompile(
            fs.readFileSync(input, 'utf-8'),
            opts.name || input,
            env
        ) );
    }
    else if(pathStats.isDirectory()) {
        addTemplates(input);

        for(var i=0; i<templates.length; i++) {
            var name = templates[i].replace(path.join(input, '/'), '');

            try {
                precompiled.push( _precompile(
                    fs.readFileSync(templates[i], 'utf-8'),
                    name,
                    env
                ) );
            } catch(e) {
                if(opts.force) {
                    // Don't stop generating the output if we're
                    // forcing compilation.
                    console.error(e);
                }
                else {
                    throw e;
                }
            }
        }
    }

    return wrapper(precompiled, opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.precompile.precompileString"></a>[function <span class="apidocSignatureSpan">nunjucks.precompile.</span>precompileString (str, opts)](#apidoc.element.nunjucks.precompile.precompileString)
- description and source-code
```javascript
function precompileString(str, opts) {
    opts = opts || {};
    opts.isString = true;
    return precompile(str, opts);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.runtime"></a>[module nunjucks.runtime](#apidoc.module.nunjucks.runtime)

#### <a name="apidoc.element.nunjucks.runtime.Frame"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>Frame ()](#apidoc.element.nunjucks.runtime.Frame)
- description and source-code
```javascript
Frame = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        var frame = new Frame();
	        this.emitLines(
	            'var ' + funcId + ' = runtime.makeMacro(',
	            '[' + argNames.join(', ') + '], ',
	            '[' + kwargNames.join(', ') + '], ',
	            'function (' + realNames.join(', ') + ') {',
	            'var callerFrame = frame;',
	            'frame = new runtime.Frame();',
	            'kwargs = kwargs || {};',
	            'if (kwargs.hasOwnProperty("caller")) {',
	            'frame.set("caller", kwargs.caller); }'
	        );

	        // Expose the arguments to the template. Don't need to use
	        // random names because the function
...
```

#### <a name="apidoc.element.nunjucks.runtime.SafeString"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>SafeString (val)](#apidoc.element.nunjucks.runtime.SafeString)
- description and source-code
```javascript
function SafeString(val) {
    if(typeof val !== 'string') {
        return val;
    }

    this.val = val;
    this.length = val.length;
}
```
- example usage
```shell
...
	        this.pushBufferId(bufferId);

	        this.withScopedSyntax(function () {
	          this.compile(node.body, frame);
	        });

	        this.emitLine('frame = callerFrame;');
	        this.emitLine('return new runtime.SafeString(' + bufferId + ');');
	        this.emitLine('});');
	        this.popBufferId();

	        return funcId;
	    },

	    compileMacro: function(node, frame) {
...
```

#### <a name="apidoc.element.nunjucks.runtime.asyncAll"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>asyncAll (arr, dimen, func, cb)](#apidoc.element.nunjucks.runtime.asyncAll)
- description and source-code
```javascript
function asyncAll(arr, dimen, func, cb) {
    var finished = 0;
    var len, i;
    var outputArr;

    function done(i, output) {
        finished++;
        outputArr[i] = output;

        if(finished === len) {
            cb(null, outputArr.join(''));
        }
    }

    if(lib.isArray(arr)) {
        len = arr.length;
        outputArr = new Array(len);

        if(len === 0) {
            cb(null, '');
        }
        else {
            for(i = 0; i < arr.length; i++) {
                var item = arr[i];

                switch(dimen) {
                case 1: func(item, i, len, done); break;
                case 2: func(item[0], item[1], i, len, done); break;
                case 3: func(item[0], item[1], item[2], i, len, done); break;
                default:
                    item.push(i, done);
                    // jshint validthis: true
                    func.apply(this, item);
                }
            }
        }
    }
    else {
        var keys = lib.keys(arr);
        len = keys.length;
        outputArr = new Array(len);

        if(len === 0) {
            cb(null, '');
        }
        else {
            for(i = 0; i < keys.length; i++) {
                var k = keys[i];
                func(k, arr[k], i, len, done);
            }
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.runtime.asyncEach"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>asyncEach (arr, dimen, iter, cb)](#apidoc.element.nunjucks.runtime.asyncEach)
- description and source-code
```javascript
function asyncEach(arr, dimen, iter, cb) {
    if(lib.isArray(arr)) {
        var len = arr.length;

        lib.asyncIter(arr, function(item, i, next) {
            switch(dimen) {
            case 1: iter(item, i, len, next); break;
            case 2: iter(item[0], item[1], i, len, next); break;
            case 3: iter(item[0], item[1], item[2], i, len, next); break;
            default:
                item.push(i, next);
                iter.apply(this, item);
            }
        }, cb);
    }
    else {
        lib.asyncFor(arr, function(key, val, i, len, next) {
            iter(key, val, i, len, next);
        }, cb);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.runtime.callWrap"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>callWrap (obj, name, context, args)](#apidoc.element.nunjucks.runtime.callWrap)
- description and source-code
```javascript
function callWrap(obj, name, context, args) {
    if(!obj) {
        throw new Error('Unable to call '' + name + '', which is undefined or falsey');
    }
    else if(typeof obj !== 'function') {
        throw new Error('Unable to call '' + name + '', which is not a function');
    }

    // jshint validthis: true
    return obj.apply(context, args);
}
```
- example usage
```shell
...
	        // Keep track of line/col info at runtime by settings
	        // variables within an expression. An expression in javascript
	        // like (x, y, z) returns the last value, and x and y can be
	        // anything
	        this.emit('(lineno = ' + node.lineno +
	                  ', colno = ' + node.colno + ', ');

	        this.emit('runtime.callWrap(');
	        // Compile it as normal.
	        this._compileExpression(node.name, frame);

	        // Output the name of what we're calling so we can get friendly errors
	        // if the lookup fails.
	        this.emit(', "' + this._getNodeName(node.name).replace(/"/g, '\\"') + '", context, ');
...
```

#### <a name="apidoc.element.nunjucks.runtime.contextOrFrameLookup"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>contextOrFrameLookup (context, frame, name)](#apidoc.element.nunjucks.runtime.contextOrFrameLookup)
- description and source-code
```javascript
function contextOrFrameLookup(context, frame, name) {
    var val = frame.lookup(name);
    return (val !== undefined) ?
        val :
        context.lookup(name);
}
```
- example usage
```shell
...
	        var name = node.value;
	        var v;

	        if((v = frame.lookup(name))) {
	            this.emit(v);
	        }
	        else {
	            this.emit('runtime.contextOrFrameLookup(' +
	                      'context, frame, "' + name + '")');
	        }
	    },

	    compileGroup: function(node, frame) {
	        this._compileAggregate(node, frame, '(', ')');
	    },
...
```

#### <a name="apidoc.element.nunjucks.runtime.copySafeness"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>copySafeness (dest, target)](#apidoc.element.nunjucks.runtime.copySafeness)
- description and source-code
```javascript
function copySafeness(dest, target) {
    if(dest instanceof SafeString) {
        return new SafeString(target);
    }
    return target.toString();
}
```
- example usage
```shell
...

	        return res;
	    },

	    capitalize: function(str) {
	        str = normalize(str, '');
	        var ret = str.toLowerCase();
	        return r.copySafeness(str, ret.charAt(0).toUpperCase() + ret.slice(1));
	    },

	    center: function(str, width) {
	        str = normalize(str, '');
	        width = width || 80;

	        if(str.length >= width) {
...
```

#### <a name="apidoc.element.nunjucks.runtime.ensureDefined"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>ensureDefined (val, lineno, colno)](#apidoc.element.nunjucks.runtime.ensureDefined)
- description and source-code
```javascript
function ensureDefined(val, lineno, colno) {
    if(val === null || val === undefined) {
        throw new lib.TemplateError(
            'attempted to output null or undefined value',
            lineno + 1,
            colno + 1
        );
    }
    return val;
}
```
- example usage
```shell
...
	                    this.compileLiteral(children[i], frame);
	                    this.emitLine(';');
	                }
	            }
	            else {
	                this.emit(this.buffer + ' += runtime.suppressValue(');
	                if(this.throwOnUndefined) {
	                    this.emit('runtime.ensureDefined(');
	                }
	                this.compile(children[i], frame);
	                if(this.throwOnUndefined) {
	                    this.emit(',' + node.lineno + ',' + node.colno + ')');
	                }
	                this.emit(', env.opts.autoescape);\n');
	            }
...
```

#### <a name="apidoc.element.nunjucks.runtime.handleError"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>handleError (error, lineno, colno)](#apidoc.element.nunjucks.runtime.handleError)
- description and source-code
```javascript
function handleError(error, lineno, colno) {
    if(error.lineno) {
        return error;
    }
    else {
        return new lib.TemplateError(error, lineno, colno);
    }
}
```
- example usage
```shell
...
	    emitFuncEnd: function(noReturn) {
	        if(!noReturn) {
	            this.emitLine('cb(null, ' + this.buffer +');');
	        }

	        this.closeScopeLevels();
	        this.emitLine('} catch (e) {');
	        this.emitLine('  cb(runtime.handleError(e, lineno, colno));');
	        this.emitLine('}');
	        this.emitLine('}');
	        this.buffer = null;
	    },

	    addScopeLevel: function() {
	        this.scopeClosers += '})';
...
```

#### <a name="apidoc.element.nunjucks.runtime.inOperator"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>inOperator (key, val)](#apidoc.element.nunjucks.runtime.inOperator)
- description and source-code
```javascript
inOperator = function (key, val) {
    if (exports.isArray(val)) {
        return exports.indexOf(val, key) !== -1;
    } else if (exports.isObject(val)) {
        return key in val;
    } else if (exports.isString(val)) {
        return val.indexOf(key) !== -1;
    } else {
        throw new Error('Cannot use "in" operator to search for "'
            + key + '" in unexpected types.');
    }
}
```
- example usage
```shell
...
	            this.compile(node.else_, frame);
	        else
	            this.emit('""');
	        this.emit(')');
	    },

	    compileIn: function(node, frame) {
	      this.emit('runtime.inOperator(');
	      this.compile(node.left, frame);
	      this.emit(',');
	      this.compile(node.right, frame);
	      this.emit(')');
	    },

	    compileOr: binOpEmitter(' || '),
...
```

#### <a name="apidoc.element.nunjucks.runtime.isArray"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>isArray ()](#apidoc.element.nunjucks.runtime.isArray)
- description and source-code
```javascript
function isArray() { [native code] }
```
- example usage
```shell
...
	            }
	        }
	        return keys;
	    }
	};

	exports.inOperator = function (key, val) {
	    if (exports.isArray(val)) {
	        return exports.indexOf(val, key) !== -1;
	    } else if (exports.isObject(val)) {
	        return key in val;
	    } else if (exports.isString(val)) {
	        return val.indexOf(key) !== -1;
	    } else {
	        throw new Error('Cannot use "in" operator to search for "'
...
```

#### <a name="apidoc.element.nunjucks.runtime.keys"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>keys (obj)](#apidoc.element.nunjucks.runtime.keys)
- description and source-code
```javascript
keys = function (obj) {
    if(Object.prototype.keys) {
        return obj.keys();
    }
    else {
        var keys = [];
        for(var k in obj) {
            if(obj.hasOwnProperty(k)) {
                keys.push(k);
            }
        }
        return keys;
    }
}
```
- example usage
```shell
...
	        }
	    }

	    next();
	};

	exports.asyncFor = function(obj, iter, cb) {
	    var keys = exports.keys(obj);
	    var len = keys.length;
	    var i = -1;

	    function next() {
	        i++;
	        var k = keys[i];
...
```

#### <a name="apidoc.element.nunjucks.runtime.makeKeywordArgs"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>makeKeywordArgs (obj)](#apidoc.element.nunjucks.runtime.makeKeywordArgs)
- description and source-code
```javascript
function makeKeywordArgs(obj) {
    obj.__keywords = true;
    return obj;
}
```
- example usage
```shell
...
	    compileKeywordArgs: function(node, frame) {
	        var names = [];

	        lib.each(node.children, function(pair) {
	            names.push(pair.key.value);
	        });

	        this.emit('runtime.makeKeywordArgs(');
	        this.compileDict(node, frame);
	        this.emit(')');
	    },

	    compileSet: function(node, frame) {
	        var ids = [];
...
```

#### <a name="apidoc.element.nunjucks.runtime.makeMacro"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>makeMacro (argNames, kwargNames, func)](#apidoc.element.nunjucks.runtime.makeMacro)
- description and source-code
```javascript
function makeMacro(argNames, kwargNames, func) {
    return function() {
        var argCount = numArgs(arguments);
        var args;
        var kwargs = getKeywordArgs(arguments);
        var i;

        if(argCount > argNames.length) {
            args = Array.prototype.slice.call(arguments, 0, argNames.length);

            // Positional arguments that should be passed in as
            // keyword arguments (essentially default values)
            var vals = Array.prototype.slice.call(arguments, args.length, argCount);
            for(i = 0; i < vals.length; i++) {
                if(i < kwargNames.length) {
                    kwargs[kwargNames[i]] = vals[i];
                }
            }

            args.push(kwargs);
        }
        else if(argCount < argNames.length) {
            args = Array.prototype.slice.call(arguments, 0, argCount);

            for(i = argCount; i < argNames.length; i++) {
                var arg = argNames[i];

                // Keyword arguments that should be passed as
                // positional arguments, i.e. the caller explicitly
                // used the name of a positional arg
                args.push(kwargs[arg]);
                delete kwargs[arg];
            }

            args.push(kwargs);
        }
        else {
            args = arguments;
        }

        return func.apply(this, args);
    };
}
```
- example usage
```shell
...
	        for(var i = 0; i < arr.length; i++) {
	            sum += arr[i];
	        }

	        return sum;
	    },

	    sort: r.makeMacro(['value', 'reverse', 'case_sensitive', 'attribute'], [], function(arr, reverse, caseSens, attr) {
	         // Copy it
	        arr = lib.map(arr, function(v) { return v; });

	        arr.sort(function(a, b) {
	            var x, y;

	            if(attr) {
...
```

#### <a name="apidoc.element.nunjucks.runtime.markSafe"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>markSafe (val)](#apidoc.element.nunjucks.runtime.markSafe)
- description and source-code
```javascript
function markSafe(val) {
    var type = typeof val;

    if(type === 'string') {
        return new SafeString(val);
    }
    else if(type !== 'function') {
        return val;
    }
    else {
        return function() {
            var ret = val.apply(this, arguments);

            if(typeof ret === 'string') {
                return new SafeString(ret);
            }

            return ret;
        };
    }
}
```
- example usage
```shell
...
	    },

	    escape: function(str) {
	        if(str instanceof r.SafeString) {
	            return str;
	        }
	        str = (str === null || str === undefined) ? '' : str;
	        return r.markSafe(lib.escape(str.toString()));
	    },

	    safe: function(str) {
	        if (str instanceof r.SafeString) {
	            return str;
	        }
	        str = (str === null || str === undefined) ? '' : str;
...
```

#### <a name="apidoc.element.nunjucks.runtime.memberLookup"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>memberLookup (obj, val)](#apidoc.element.nunjucks.runtime.memberLookup)
- description and source-code
```javascript
function memberLookup(obj, val) {
    obj = obj || {};

    if(typeof obj[val] === 'function') {
        return function() {
            return obj[val].apply(obj, arguments);
        };
    }

    return obj[val];
}
```
- example usage
```shell
...
	            var n = node.ops[i];
	            this.emit(' ' + compareOps[n.type] + ' ');
	            this.compile(n.expr, frame);
	        }
	    },

	    compileLookupVal: function(node, frame) {
	        this.emit('runtime.memberLookup((');
	        this._compileExpression(node.target, frame);
	        this.emit('),');
	        this._compileExpression(node.val, frame);
	        this.emit(')');
	    },

	    _getNodeName: function(node) {
...
```

#### <a name="apidoc.element.nunjucks.runtime.numArgs"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>numArgs (args)](#apidoc.element.nunjucks.runtime.numArgs)
- description and source-code
```javascript
function numArgs(args) {
    var len = args.length;
    if(len === 0) {
        return 0;
    }

    var lastArg = args[len - 1];
    if(lastArg && lastArg.hasOwnProperty('__keywords')) {
        return len - 1;
    }
    else {
        return len;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.runtime.suppressValue"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>suppressValue (val, autoescape)](#apidoc.element.nunjucks.runtime.suppressValue)
- description and source-code
```javascript
function suppressValue(val, autoescape) {
    val = (val !== undefined && val !== null) ? val : '';

    if(autoescape && !(val instanceof SafeString)) {
        val = lib.escape(val.toString());
    }

    return val;
}
```
- example usage
```shell
...

	    compileCallExtension: function(node, frame, async) {
	        var args = node.args;
	        var contentArgs = node.contentArgs;
	        var autoescape = typeof node.autoescape === 'boolean' ? node.autoescape : true;

	        if(!async) {
	            this.emit(this.buffer + ' += runtime.suppressValue(');
	        }

	        this.emit('env.getExtension("' + node.extName + '")["' + node.prop + '"](');
	        this.emit('context');

	        if(args || contentArgs) {
	            this.emit(',');
...
```



# <a name="apidoc.module.nunjucks.runtime.Frame"></a>[module nunjucks.runtime.Frame](#apidoc.module.nunjucks.runtime.Frame)

#### <a name="apidoc.element.nunjucks.runtime.Frame.Frame"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>Frame ()](#apidoc.element.nunjucks.runtime.Frame.Frame)
- description and source-code
```javascript
Frame = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        var frame = new Frame();
	        this.emitLines(
	            'var ' + funcId + ' = runtime.makeMacro(',
	            '[' + argNames.join(', ') + '], ',
	            '[' + kwargNames.join(', ') + '], ',
	            'function (' + realNames.join(', ') + ') {',
	            'var callerFrame = frame;',
	            'frame = new runtime.Frame();',
	            'kwargs = kwargs || {};',
	            'if (kwargs.hasOwnProperty("caller")) {',
	            'frame.set("caller", kwargs.caller); }'
	        );

	        // Expose the arguments to the template. Don't need to use
	        // random names because the function
...
```

#### <a name="apidoc.element.nunjucks.runtime.Frame.extend"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.</span>extend (name, props)](#apidoc.element.nunjucks.runtime.Frame.extend)
- description and source-code
```javascript
extend = function (name, props) {
    if(typeof name === 'object') {
        props = name;
        name = 'anonymous';
    }
    return extend(new_cls, name, props);
}
```
- example usage
```shell
...

	// If the user is using the async API, *always* call it
	// asynchronously even if the template was synchronous.
	function callbackAsap(cb, err, res) {
	    asap(function() { cb(err, res); });
	}

	var Environment = Obj.extend({
	    init: function(loaders, opts) {
	        // The dev flag determines the trace that'll be shown on errors.
	        // If set to true, returns the full trace from the error point,
	        // otherwise will return trace starting from Template.render
	        // (the full trace from within nunjucks may confuse developers using
	        //  the library)
	        // defaults to false
...
```



# <a name="apidoc.module.nunjucks.runtime.Frame.prototype"></a>[module nunjucks.runtime.Frame.prototype](#apidoc.module.nunjucks.runtime.Frame.prototype)

#### <a name="apidoc.element.nunjucks.runtime.Frame.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.prototype.</span>constructor ()](#apidoc.element.nunjucks.runtime.Frame.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.runtime.Frame.prototype.get"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.prototype.</span>get (name)](#apidoc.element.nunjucks.runtime.Frame.prototype.get)
- description and source-code
```javascript
get = function (name) {
    var val = this.variables[name];
    if(val !== undefined) {
        return val;
    }
    return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.runtime.Frame.prototype.init"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.prototype.</span>init (parent, isolateWrites)](#apidoc.element.nunjucks.runtime.Frame.prototype.init)
- description and source-code
```javascript
init = function (parent, isolateWrites) {
    this.variables = {};
    this.parent = parent;
    this.topLevel = false;
    // if this is true, writes (set) should never propagate upwards past
    // this frame to its parent (though reads may).
    this.isolateWrites = isolateWrites;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nunjucks.runtime.Frame.prototype.lookup"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.prototype.</span>lookup (name)](#apidoc.element.nunjucks.runtime.Frame.prototype.lookup)
- description and source-code
```javascript
lookup = function (name) {
    var p = this.parent;
    var val = this.variables[name];
    if(val !== undefined) {
        return val;
    }
    return p && p.lookup(name);
}
```
- example usage
```shell
...

	    lookup: function(name) {
	        var p = this.parent;
	        var val = this.variables[name];
	        if(val !== undefined) {
	            return val;
	        }
	        return p && p.lookup(name);
	    },

	    resolve: function(name, forWrite) {
	        var p = (forWrite && this.isolateWrites) ? undefined : this.parent;
	        var val = this.variables[name];
	        if(val !== undefined) {
	            return this;
...
```

#### <a name="apidoc.element.nunjucks.runtime.Frame.prototype.pop"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.prototype.</span>pop ()](#apidoc.element.nunjucks.runtime.Frame.prototype.pop)
- description and source-code
```javascript
pop = function () {
    return this.parent;
}
```
- example usage
```shell
...
	 * @param {{call}} task A callable object, typically a function that takes no
	 * arguments.
	 */
	module.exports = asap;
	function asap(task) {
	    var rawTask;
	    if (freeTasks.length) {
	        rawTask = freeTasks.pop();
	    } else {
	        rawTask = new RawTask();
	    }
	    rawTask.task = task;
	    rawAsap(rawTask);
	}
...
```

#### <a name="apidoc.element.nunjucks.runtime.Frame.prototype.push"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.prototype.</span>push (isolateWrites)](#apidoc.element.nunjucks.runtime.Frame.prototype.push)
- description and source-code
```javascript
push = function (isolateWrites) {
    return new Frame(this, isolateWrites);
}
```
- example usage
```shell
...

	exports.groupBy = function(obj, val) {
	    var result = {};
	    var iterator = exports.isFunction(val) ? val : function(obj) { return obj[val]; };
	    for(var i=0; i<obj.length; i++) {
	        var value = obj[i];
	        var key = iterator(value, i);
	        (result[key] || (result[key] = [])).push(value);
	    }
	    return result;
	};

	exports.toArray = function(obj) {
	    return Array.prototype.slice.call(obj);
	};
...
```

#### <a name="apidoc.element.nunjucks.runtime.Frame.prototype.resolve"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.prototype.</span>resolve (name, forWrite)](#apidoc.element.nunjucks.runtime.Frame.prototype.resolve)
- description and source-code
```javascript
resolve = function (name, forWrite) {
    var p = (forWrite && this.isolateWrites) ? undefined : this.parent;
    var val = this.variables[name];
    if(val !== undefined) {
        return this;
    }
    return p && p.resolve(name);
}
```
- example usage
```shell
...
	            throw new Error('filter not found: ' + name);
	        }
	        return this.filters[name];
	    },

	    resolveTemplate: function(loader, parentName, filename) {
	        var isRelative = (loader.isRelative && parentName)? loader.isRelative(filename) : false;
	        return (isRelative && loader.resolve)? loader.resolve(parentName, filename) : filename;
	    },

	    getTemplate: function(name, eagerCompile, parentName, ignoreMissing, cb) {
	        var that = this;
	        var tmpl = null;
	        if(name && name.raw) {
	            // this fixes autoescape for templates referenced in symbols
...
```

#### <a name="apidoc.element.nunjucks.runtime.Frame.prototype.set"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.Frame.prototype.</span>set (name, val, resolveUp)](#apidoc.element.nunjucks.runtime.Frame.prototype.set)
- description and source-code
```javascript
set = function (name, val, resolveUp) {
    // Allow variables with dots by automatically creating the
    // nested structure
    var parts = name.split('.');
    var obj = this.variables;
    var frame = this;

    if(resolveUp) {
        if((frame = this.resolve(parts[0], true))) {
            frame.set(name, val);
            return;
        }
    }

    for(var i=0; i<parts.length - 1; i++) {
        var id = parts[i];

        if(!obj[id]) {
            obj[id] = {};
        }
        obj = obj[id];
    }

    obj[parts[parts.length - 1]] = val;
}
```
- example usage
```shell
...
	            if (!this.ext) this.name += (this.ext = ('.' !== this.defaultEngine[0] ? '.' : '') + this.defaultEngine);
	        }

	        NunjucksView.prototype.render = function(opts, cb) {
	          env.render(this.name, opts, cb);
	        };

	        app.set('view', NunjucksView);
	        app.set('nunjucksEnv', this);
	        return this;
	    },

	    render: function(name, ctx, cb) {
	        if(lib.isFunction(ctx)) {
	            cb = ctx;
...
```



# <a name="apidoc.module.nunjucks.runtime.SafeString"></a>[module nunjucks.runtime.SafeString](#apidoc.module.nunjucks.runtime.SafeString)

#### <a name="apidoc.element.nunjucks.runtime.SafeString.SafeString"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.</span>SafeString (val)](#apidoc.element.nunjucks.runtime.SafeString.SafeString)
- description and source-code
```javascript
function SafeString(val) {
    if(typeof val !== 'string') {
        return val;
    }

    this.val = val;
    this.length = val.length;
}
```
- example usage
```shell
...
	        this.pushBufferId(bufferId);

	        this.withScopedSyntax(function () {
	          this.compile(node.body, frame);
	        });

	        this.emitLine('frame = callerFrame;');
	        this.emitLine('return new runtime.SafeString(' + bufferId + ');');
	        this.emitLine('});');
	        this.popBufferId();

	        return funcId;
	    },

	    compileMacro: function(node, frame) {
...
```



# <a name="apidoc.module.nunjucks.runtime.SafeString.prototype"></a>[module nunjucks.runtime.SafeString.prototype](#apidoc.module.nunjucks.runtime.SafeString.prototype)

#### <a name="apidoc.element.nunjucks.runtime.SafeString.prototype.toString"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.SafeString.prototype.</span>toString ()](#apidoc.element.nunjucks.runtime.SafeString.prototype.toString)
- description and source-code
```javascript
toString = function () {
    return this.val;
}
```
- example usage
```shell
...
	    },

	    escape: function(str) {
	        if(str instanceof r.SafeString) {
	            return str;
	        }
	        str = (str === null || str === undefined) ? '' : str;
	        return r.markSafe(lib.escape(str.toString()));
	    },

	    safe: function(str) {
	        if (str instanceof r.SafeString) {
	            return str;
	        }
	        str = (str === null || str === undefined) ? '' : str;
...
```

#### <a name="apidoc.element.nunjucks.runtime.SafeString.prototype.valueOf"></a>[function <span class="apidocSignatureSpan">nunjucks.runtime.SafeString.prototype.</span>valueOf ()](#apidoc.element.nunjucks.runtime.SafeString.prototype.valueOf)
- description and source-code
```javascript
valueOf = function () {
    return this.val;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nunjucks.transformer"></a>[module nunjucks.transformer](#apidoc.module.nunjucks.transformer)

#### <a name="apidoc.element.nunjucks.transformer.transform"></a>[function <span class="apidocSignatureSpan">nunjucks.transformer.</span>transform (ast, asyncFilters)](#apidoc.element.nunjucks.transformer.transform)
- description and source-code
```javascript
function transform(ast, asyncFilters) {
    return cps(ast, asyncFilters || []);
}
```
- example usage
```shell
...
	    }
	});

	// var c = new Compiler();
	// var src = 'hello {% filter title %}' +
	//     'Hello madam how are you' +
	//     '{% endfilter %}'
	// var ast = transformer.transform(parser.parse(src));
	// nodes.printNodes(ast);
	// c.compile(ast);
	// var tmpl = c.getCode();
	// console.log(tmpl);

	module.exports = {
	    compile: function(src, asyncFilters, extensions, name, opts) {
...
```



# <a name="apidoc.module.nunjucks.web_loaders"></a>[module nunjucks.web_loaders](#apidoc.module.nunjucks.web_loaders)

#### <a name="apidoc.element.nunjucks.web_loaders.PrecompiledLoader"></a>[function <span class="apidocSignatureSpan">nunjucks.web_loaders.</span>PrecompiledLoader ()](#apidoc.element.nunjucks.web_loaders.PrecompiledLoader)
- description and source-code
```javascript
PrecompiledLoader = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
	        }

	        // It's easy to use precompiled templates: just include them
	        // before you configure nunjucks and this will automatically
	        // pick it up and use it
	        if((true) && window.nunjucksPrecompiled) {
	            this.loaders.unshift(
	                new builtin_loaders.PrecompiledLoader(window.nunjucksPrecompiled)
	            );
	        }

	        this.initCache();

	        this.globals = globals();
	        this.filters = {};
...
```

#### <a name="apidoc.element.nunjucks.web_loaders.WebLoader"></a>[function <span class="apidocSignatureSpan">nunjucks.web_loaders.</span>WebLoader ()](#apidoc.element.nunjucks.web_loaders.WebLoader)
- description and source-code
```javascript
WebLoader = function () {
    if(prototype.init) {
        prototype.init.apply(this, arguments);
    }
}
```
- example usage
```shell
...
if(loaders.FileSystemLoader) {
    TemplateLoader = new loaders.FileSystemLoader(templatesPath, {
        watch: opts.watch,
        noCache: opts.noCache
    });
}
else if(loaders.WebLoader) {
    TemplateLoader = new loaders.WebLoader(templatesPath, {
        useCache: opts.web && opts.web.useCache,
        async: opts.web && opts.web.async
    });
}

e = new env.Environment(TemplateLoader, opts);
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
