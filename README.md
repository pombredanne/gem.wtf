# gem.wtf

Type a short URL to jump straight to a Ruby gem's repository page.

## Examples

- [gem.wtf/nokogiri](https://gem.wtf/nokogiri)
- [gem.wtf/faker](https://gem.wtf/faker)
- [gem.wtf/rails](https://gem.wtf/rails)
- [gem.wtf/gemoji](https://gem.wtf/gemoji)
- [gem.wtf/stamp](https://gem.wtf/stamp)

## How it Works

- A request is made to the [RubyGems.org API](https://guides.rubygems.org/rubygems-org-api/) to fetch the gem's metdata, e.g. [rubygems.org/api/v1/gems/rails.json](https://rubygems.org/api/v1/gems/rails.json)
- If a `source_code_uri` is in the metadata, you'll be redirected to it.
- If a `documentation_uri` is in the metadata, you'll be redirected to it.
- If neither of those are present, you'll be redirected to `rubygems.org/gems/<gem-name>`

## License

MIT