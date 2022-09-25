# openapi-generator-custom-practice


OpenApi generatorを使用した自動生成コードを作成する。
  
https://github.com/OpenAPITools/openapi-generator


# 動いたやつ

javaのspringは素直にspringでいいらしい。

```bash
java -jar libs/openapi-generator-cli-6.2.0.jar generate \
   -i https://raw.githubusercontent.com/openapitools/openapi-generator/master/modules/openapi-generator/src/test/resources/3_0/petstore.yaml \
   -g spring \
   -o output/spring \
   -t templates/JavaSpring
```

※ swagger codegenの場合、javaSpringだった気がする。


```bash
# help?
java -jar libs/openapi-generator-cli-6.2.0.jar help generate
```

-  springの生成時の使い方
    - https://github.com/OpenAPITools/openapi-generator/blob/master/docs/generators/spring.md
- 公式側で用意しているテンプレート
    - https://github.com/OpenAPITools/openapi-generator/tree/master/modules/openapi-generator/src/main/resources/JavaSpring


# 動かないやつ
```bash
# 公式に記載してあったDocker生成方法
# ※ Windowsだとうまく動かない？
docker run --rm -v "${PWD}:/local" openapitools/openapi-generator-cli generate \
    -i https://raw.githubusercontent.com/openapitools/openapi-generator/master/modules/openapi-generator/src/test/resources/3_0/petstore.yaml \
    -g go \
    -o "/local/out/go"
```

# 参考記事

- swagger Codegenの説明だけど、同じようにできる
    - https://qiita.com/Quramy/items/c583f3213f0b77ff1bac