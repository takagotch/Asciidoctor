### Asciidoctor
---
https://github.com/asciidoctor/asciidoctor

```ruby
asciidoctor --version
asciidoctor README.md
asciidoctor --help
asciidoctor -D output README.adoc


require 'asciidoctor'
Asciidoctor.convert_file 'README.adoc', to_file: true, safe: :safe

convert = '_Zen_ in the art of writing https://asciidoctor.org[AsciiDoc].'
Asciidoctor.convert content, safe: :safe

content = '_Zen_ in the art of writing https://asciidoctor.org[AsciiDoc]'
html = Asciidoctor.convert content, header_footer: true, safe: :safe

content = '_Zen_ in the art of writing https://asciidoctor.org[AsciiDoc]'
document = Asciidoctor.load content, header_footer: true, safe: :safe
puts = document.convert
html = document.convert
```

