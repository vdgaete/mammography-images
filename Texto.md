# Análise de mamografias utilizando redes neurais convolucionais

## Introdução

O câncer de mama é o segundo tipo de câncer mais comum entre as mulheres no mundo e no Brasil, ficando atrás apenas do câncer de pele não melanoma. De acordo com o Instituto Nacional de Câncer (INCA), em 2018, foram estimados 59.700 novos casos de câncer de mama no Brasil, com um risco estimado de 56,33 casos a cada 100 mil mulheres. O câncer de mama também acomete homens, porém é raro, representando apenas 1% do total de casos da doença. 

O diagnóstico precoce é um fator importante para o sucesso do tratamento e cura do câncer de mama. O autoexame é uma forma de detecção precoce, porém não é considerado um método eficaz para o diagnóstico da doença. O exame clínico e a mamografia são os métodos mais eficazes para o diagnóstico precoce do câncer de mama.

Entretanto, a mamografia é um exame que pode apresentar resultados falsos positivos, ou seja, o exame pode indicar a presença de câncer de mama quando na verdade não há. Isso pode gerar ansiedade e preocupação desnecessária para a paciente, além de gerar custos para o sistema de saúde. Por outro lado, o exame também pode apresentar resultados falsos negativos, ou seja, o exame pode indicar que não há câncer de mama quando na verdade há. Isso pode atrasar o diagnóstico e tratamento da doença, o que pode diminuir as chances de cura da paciente.

A mamografia é um exame que gera imagens do interior da mama, que são analisadas por um médico radiologista. A análise das imagens é um processo demorado e que requer atenção e concentração do médico. Por isso, a utilização de sistemas computacionais para auxiliar o médico radiologista na análise das imagens de mamografia pode ser uma alternativa para melhorar a eficiência do diagnóstico.

## Objetivo

O objetivo deste trabalho é analisar a influência de filtros de contrastraste e de técnicas de pré-processamento de imagens na classificação de mamografias utilizando redes neurais convolucionais, a fim de verificar se essas técnicas podem melhorar a acurácia do modelo de classificação.

## Metodologia

Para a realização deste trabalho, foi utilizado o dataset CBIS-DDSM (Curated Breast Imaging Subset of DDSM), que é um subconjunto do DDSM (Digital Database for Screening Mammography), que é um dataset de mamografias digitais. O CBIS-DDSM é composto por 2.620 mamografias, sendo 1.535 mamografias benignas e 1.085 mamografias malignas. O dataset está disponível em: https://wiki.cancerimagingarchive.net/display/Public/CBIS-DDSM.

O dataset CBIS-DDSM é composto por 4 tipos de imagens: crânio-caudal (CC), médio-lateral oblíqua (MLO), crânio-caudal com compressão (CC with compression) e médio-lateral oblíqua com compressão (MLO with compression). As imagens CC e MLO são imagens de mamografias sem compressão, enquanto as imagens CC with compression e MLO with compression são imagens de mamografias com compressão. As imagens com compressão são utilizadas para a detecção de microcalcificações, enquanto as imagens sem compressão são utilizadas para a detecção de massas.

O dataset é separado em 2 categorias, calcificações e massas, cada categoria apresenta os conjuntos de testes e treinamento separados.


As imagens foram convertidas para escala de cinza e foram aplicados filtros de contraste nas imagens. Foram utilizados 3 filtros de contraste: filtro de contraste de histograma, filtro de contraste de equalização de histograma e filtro de contraste adaptativo de histograma. As imagens foram pré-processadas utilizando 3 técnicas: normalização, equalização de histograma e equalização de histograma adaptativa.

Para a classificação das imagens, foram utilizadas redes neurais convolucionais. Foram utilizadas 3 arquiteturas de redes neurais convolucionais: VGG19, ResNet50 e InceptionV3. As redes neurais convolucionais foram inicializadas com os pesos pré-treinados no dataset ImageNet. As redes neurais convolucionais foram treinadas utilizando o conjunto de treinamento e validação. Após o treinamento, as redes neurais convolucionais foram avaliadas utilizando o conjunto de teste.

Será proposto diferentes combinações de filtros de contraste e de técnicas de pré-processamento de imagens para verificar se essas técnicas podem melhorar a acurácia do modelo de classificação, e analisar a influência técnicas, baseados nas métricas escolhidas.

As combinções de filtros de contraste e de técnicas de pré-processamento de imagens serão avaliadas e comparadas com resultados obtidos sem a utilização de filtros de contraste e de técnicas de pré-processamento de imagens.

## Resultados

Os resultados obtidos com a utilização de filtros de contraste e de técnicas de pré-processamento de imagens serão comparados com os resultados obtidos sem a utilização de filtros de contraste e de técnicas de pré-processamento de imagens.

## Conclusão

Os resultados obtidos com a utilização de filtros de contraste e de técnicas de pré-processamento de imagens serão comparados com os resultados obtidos sem a utilização de filtros de contraste e de técnicas de pré-processamento de imagens.

## Referências

- https://www.inca.gov.br/tipos-de-cancer/cancer-de-mama
- https://www.inca.gov.br/sites/ufu.sti.inca.local/files//media/document//cancer-de-mama-2018.pdf

