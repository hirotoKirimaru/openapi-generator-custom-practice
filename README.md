# openapi-generator-custom-practice


OpenApi generatorを使用した自動生成コードを作成する。
  
https://github.com/OpenAPITools/openapi-generator





# 動かないやつ
```bash
# 公式に記載してあったDocker生成方法
# ※ Windowsだとうまく動かない？
docker run --rm -v "${PWD}:/local" openapitools/openapi-generator-cli generate \
    -i https://raw.githubusercontent.com/openapitools/openapi-generator/master/modules/openapi-generator/src/test/resources/3_0/petstore.yaml \
    -g go \
    -o "/local/out/go"
```
