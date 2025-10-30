TODO:

Elementy do wykonania ręcznie po poprawnym wykonaniu się całego skryptu:

1) Instalacja Fleet'a - instalowany na sondzie - do wykonania wszystko według guide'a, który jest generowany w Kibanie; należy pamiętać o w skazaniu certyfikatów oraz zmianie adresu elasticsearcha (domyślnie ma http://localhost:9200 a ma mieć https://<adres_ip_sondy>:9200)
2) We Fleet w Settings należy skonfigurować output do elastica - dodać odpowiedni adres, oraz dodać certyfikat
  ssl:
    certificate_authorities: ["path/to/ca.crt"]
3) Instalacja Agentów - należy upewnic się, że serwer/stacja robocza, na której instalujemy agenta ufa certyfikatowi ca.crt. W razie problemów z zaufaniem certyfikatowi można dodać "--insecure" na końcu komendy do instalacji/enrollowania
