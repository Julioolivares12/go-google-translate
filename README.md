go-google-translate


install

go get github.com/Julioolivares12/go-google-translate

example

import (
    "github.com/Julioolivares12/google-translate/traductor"
    "fmt"
)
func main() {
    r , err := traductor.Translate("es", "en", "hola")
    if err != nil{
      panic(err)
    }
    fmt.Println(r.Sentences[0].Trans)
}
