# For-you-tathia
website ini di buat untuk kamuu seorang dengan penuh kasih sayanggg
hidden=[".config"]

# hosting is currently hardcoded for this language
# [hosting]
# route = "/"
# directory= "/"

[nix]
channel = "stable-21_11"

[languages.html]
pattern = "**/*.html"
  [languages.html.languageServer]
  start = ["vscode-html-language-server", "--stdio"]
  [languages.html.languageServer.initializationOptions]
  provideFormatter = true
  [languages.html.languageServer.configuration.html]
  customData = [ ]
  autoCreateQuotes = true
  autoClosingTags = true
  mirrorCursorOnMatchingTag = false
  
    [languages.html.languageServer.configuration.html.completion]
    attributeDefaultValue = "doublequotes"
  
    [languages.html.languageServer.configuration.html.format]
    enable = true
    wrapLineLength = 120
    unformatted = "wbr"
    contentUnformatted = "pre,code,textarea"
    indentInnerHtml = false
    preserveNewLines = true
    indentHandlebars = false
    endWithNewline = false
    extraLiners = "head, body, /html"
    wrapAttributes = "auto"
    templating = false
    unformattedContentDelimiter = ""
  
    [languages.html.languageServer.configuration.html.suggest]
    html5 = true
  
    [languages.html.languageServer.configuration.html.validate]