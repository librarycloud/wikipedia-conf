# wikipedia nginx conf
代理维基全站，基于lnmp.org的nginx配置。
nginx要添加`ngx_brotli`model。
* 详细教程[Debian](https://github.com/librarycloud/iwiki/wiki/Debian-%E8%AF%A6%E7%BB%86%E6%90%AD%E5%BB%BA%E6%95%99%E7%A8%8B)
## 使用方法(假设你的域名为 `abc.com` )：
1. 将`{$domain2}`替换为`abc`，将`{$domain1}`替换为`com`
2. ssl证书需要申请以下域名（dns同样需要添加解析记录）
```
*.abc.com
*.wikimedia.abc.com
*.wikipedia.abc.com
*.wikimediafoundation.abc.com
*.wiktionary.abc.com
*.wikivoyage.abc.com
*.wikiversity.abc.com
*.wikisource.abc.com
*.wikiquote.abc.com
*.wikinews.abc.com
*.wikidata.abc.com
*.mediawiki.abc.com
*.wikibooks.abc.com
*.m.wikimedia.abc.com
*.m.wikipedia.abc.com
*.m.wmfusercontent.abc.com
*.m.wikimediafoundation.abc.com
*.m.wiktionary.abc.com
*.m.wikivoyage.abc.com
*.m.wikiversity.abc.com
*.m.wikisource.abc.com
*.m.wikiquote.abc.com
*.m.wikinews.abc.com
*.m.wikidata.abc.com
*.m.mediawiki.abc.com
*.m.wikibooks.abc.com
*.wmfusercontent.abc.com
```

部分dns（例如aliyun）的解析记录还需添加所有去除`*.`的记录。
## 参考：
> + https://github.com/AnYiEE/nginx-wikimirror
> + https://github.com/imlinhanchao/ngx_proxy_wiki
