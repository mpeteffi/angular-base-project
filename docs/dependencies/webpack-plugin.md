# Webpack Plugin

  Os plugins do webpack servem para adicionar ações ao empacotar os arquivos.

-- clean-webpack-plugin
  Limpa o diretório onde os arquivos empacotados serão empacotados no build. Dessa forma, evitando problemas que possam ser causados por sobrescrita de arquivos.

-- extract-text-webpack-plugin
  Extrai todo conteúdo de um determinado tipo de arquivo para um arquivo único. Nesse caso, estamos usando para CSS.

-- UglifyJsPlugin
	É o plugin que vai cuidar de comprimir e minificar o arquivo JS final.
	A opção `mangle` que é passada por parâmetro, define se as variáveis terão seus nomes substituidos ou não.


Tamanho final do bundle.js para o mesmo projeto:
1.63 MB - Sem uglify.
483 kB  - Com uglify, sem trocar nome de variáveis.
286 kB  - Com Uglify e trocando nome de variáveis.
