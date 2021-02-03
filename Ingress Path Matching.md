# Ingress Path Match

(!) **Important**
Expressões regulares e curingas não são compatíveis com o campo `spec.rules.host`.


O ingress controller suporta expressões regulares que não diferenciam maiúsculas de minúsculas no campo `spec.rules.http.paths.path`


(!) **DICA**
O Kubernetes aceita apenas expressões que estejam em conformidade com a sintaxe do mecanismo RE2. É possível que expressões válidas aceitas por NGINX não possam ser usadas com ingress-nginx, porque a biblioteca PCRE (usada em NGINX) oferece suporte a uma sintaxe mais ampla que RE2. Consulte a documentação da sintaxe RE2 para obter as diferenças.

## Prioridade de caminho

No NGINX, as expressões regulares seguem uma política de primeira correspondência. Para permitir uma correspondência de caminho mais precisa, ingress-nginx primeiro ordena os caminhos por comprimento decrescente antes de gravá-los no modelo NGINX como blocos de localização.




# Referencias

Ingress Path Matching - https://kubernetes.github.io/ingress-nginx/user-guide/ingress-path-matching/#ingress-path-matching

