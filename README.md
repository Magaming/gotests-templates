# gotests-templates

custom templates for [gotests](https://github.com/cweill/gotests)

- using [go-cmp](https://github.com/google/go-cmp)
- custom error message  

  default:
  ```
    t.Errorf("`StructName`.`MethodName` = %v, want %v", got, tt.want)
  ```
  
  custom: 
  ```
    t.Errorf("`StructName`.`MethodName` got: %#v, want: %#v", got, tt.want)
  ```

## Usage in Visual Studio Code

1. Add [vscode-go] extension
1. Clone this repository
1. Add config to setting.json
  ```
  "go.generateTestsFlags": [
    "-template_dir",
    "/your_local_directory/gotests-templates/templates"
  ]
  ```
