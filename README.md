Gaia - Sistema desenvolvido para solução do Desafio 1, do 1º Hackaliods CNJ (Hackathon).
*Como melhorar o canal de comunicação da sociedade com o Judiciário (via judicial ou extrajudicial). Como podemos relatar a análise quantitativa ou qualitativa da possível existência de crimes ambientais de invasão de florestas públicas ou de terras indígenas nos municípios, por hectares, como reclamação pré-processual ou como ata notarial?*

A Gaia é um projeto desenvolvido por uma equipe multidisciplinar que tem o objetivo de auxiliar o sistema de justiça no tratamento de crimes de incêndio. A partir da notificação automatizada de focos de fogo em matas e florestas públicas às autoridades, a ferramenta dinamiza a ação do judiciário na proteção ambiental. 

Inicialmente, a ferramenta fomenta a participação da sociedade civil no desenvolvimento sustentável e na preservação dos recursos naturais, pois aprimora a notificação de crimes de incêndio às autoridades competentes. Trata-se de um projeto de iniciativa privada à serviço do direito à vida em um ambiente ecologicamente equilibrado, realizando o Princípio 10 da Declaração do Rio sobre Meio Ambiente, para além do objetivo constitucional de proteção ao meio ambiente. 

Gaia é uma ação para realizar os Objetivos de Desenvolvimento Sustentável da Agenda 2030 da ONU, especialmente o ODS 13 - Tomar medidas urgentes para combater a mudança do clima e seus impactos - e o ODS 15 - Proteger, recuperar e promover o uso sustentável dos ecossistemas terrestres, gerir de forma sustentável as florestas, combater a desertificação, deter e reverter a degradação da terra e deter a perda de biodiversidade. . 

A ferramenta funciona a partir da base de dados disponibilizada diariamente ao público pelo BDQueimadas, projeto do Programa de Queimadas do INPE. A base de dados consiste em diversas informações de focos de queimadas obtidas através das imagens de satélites. A partir desse banco é possível obter informações sobre o dia do fato, horário, município, coordenadas geográficas, área atingida, bioma afetado e órgão responsável pela fiscalização. A partir desses dados, o sistema Gaia informa também o direcionamento aproximado do foco de incêndio. 

Havendo foco de incêndio detectado pelo BDQueimadas, o sistema automaticamente gera uma notícia crime que é encaminhada ao Ministério Público Estadual competente mais próximo (através de e-mail) e, quando possível, à ouvidoria do órgão responsável pela área.. Futuramente, o sistema irá automatizar o envio da notícia crime ao Ministério Público Federal nos casos em que a queimada for registrada em terras da União.
 
Os alertas são confiáveis, porém não estão diretamente associados à realização de um crime. Nesse ponto, entra a figura do profissional do direito em avaliar a situação fática e enquadrá-las nos tipos penais para o crime de incêndio: art. 41, Lei 9.605/98; art. 41, p. u., Lei 9.605/98; art. 54, Lei 9.605/98; art. 250, Código Penal. O sistema dinamiza o Poder Judiciário sem eliminar a atuação do promotor de justiça, pois apenas busca tornar o trabalho desse agente mais eficiente.

A solução criada para o Desafio 1 irá atingir queimadas em terras públicas de ao menos 30m², conforme informações disponibilizadas pela plataforma BDQueimadas (INPE). Relatórios poderão ser gerados com informações do tamanho das queimadas e da localidade em que elas são feitas, o que tem o objetivo de melhorar o canal de comunicação da sociedade com o Judiciário (via judicial), de forma quantitativa e qualitativa.

Tecnologia utilizada

O sistema é web e foi desenvolvido em Python com o uso do framework DJango/GeoDJango. O banco de dados utilizado foi o Postgres v13, e a IDE utilizada foi o PyCharm Professional.

Os dados utilizados foram os seguintes:

Alertas de desmatamento: base DETER do INPE, pública para download.

Cadastro Nacional de Florestas Públicas: Serviço Florestal Brasileiro

Cadastro de Municípios e Unidades da Federação: IBGE

Todos os cruzamentos de dados necessários foram feitos via Postgres, com o uso da extensão PostGIS.




