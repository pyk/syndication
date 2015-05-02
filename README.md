# Syndication

`syndication` is a simple RSS & Atom feeds reader written in Go language. 

### Goal
    
    - simple, easy to use
    - using standart libs only

### Blueprint

    var content syndication.Content
    s := syndication.NewReader(io.Reader) // usually response body
    err := s.Read(&content)
    if err != nil {
        fmt.Printf("syndication.Read error: %v\n", err)
    }
    fmt.Printf("Syndication content: %#v\n", content)
