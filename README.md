## Lab4-Imagens-Biomedicas
# Laboratório 4 da disciplina de Imagens Biomédicas

No laboratório 2 da disciplina de Imagens Biomédicas, trabalhamos com algumas noções sobre aplicação de filtros de mediana, máscaras Gaussianas, "afiamento" de bordas e gradientes.

Filtro Mediana  
A imagem à esquerda foi gerada através de um exame de Ressonância Magnética e foi poluída por um ruído do tipo salt and pepper.  
A imagem à direita foi tratada por um filtro mediana com todos pesos iguais a 1.  
<p align="center">
<img src = "https://user-images.githubusercontent.com/86500603/209250177-1b0f92c2-bf6d-4dc5-bdaf-dbfdba6693ba.png" width = 300>
<img src = "https://user-images.githubusercontent.com/86500603/209250298-85d21381-b8c9-4239-b60f-b39fceb6f0ee.png" width = 300>
</p>

Filtro Gaussiano  
A imagem à esquerda representa o vetor Gaussiano utilizado para compor a máscara 2D Gaussiana.  
A imagem à direita representa a máscara 2D Gaussiana.  

<p align="center">
<img src = "https://user-images.githubusercontent.com/86500603/209250537-14b0621c-783a-4236-9946-758e7149f792.png" height = 300>
<img src = "https://user-images.githubusercontent.com/86500603/209250621-fc2d847b-0492-4d3e-931c-295ebf206739.png" height = 300>
</p>

Exemplos de aplicação de Filtro Gaussiano  
A imagem à esquerda representa uma imagem de exame de mamografia sem aplicação de filtros.  
A imagem à direita representa a mesma imagem tratada com o filtro Gaussiano anterior.  
A idéia por trás da aplicação desses filtros é alternar o contraste que a imagem possui, modelando a máscara do filtro.
<p align="center">
<img src = "https://user-images.githubusercontent.com/86500603/209254028-1c05fa3c-c3ec-4345-b8e1-0591e0f2da65.png" height = 300>
<img src = "https://user-images.githubusercontent.com/86500603/209254058-a1895def-4ff7-445f-b12d-b5bfc69e4630.png" height = 300>
</p>
  
A imagem à esquerda representa uma máscara de dimensão maior (15x15), tendo gaussiana de média 7, dp 2 e normalizada entre 0 e 1.  
A imagem à direita representa a mesma imagem tratada com o filtro Gaussiano novo.  
<p align="center">
<img src = "https://user-images.githubusercontent.com/86500603/209254231-3a590214-e879-4f53-bd45-2fed81ad2f23.png" height = 300>
<img src = "https://user-images.githubusercontent.com/86500603/209254239-97cc07fb-c514-41d2-8f82-40fca584bf67.png" height = 300>
</p>

  
Afiamento de bordas  
O afiamento de bordas é um processo que contrasta mais as bordas da imagem, os exemplos abaixo ilustram as imagens de ressonância magnética utilizadas.  
Para fazer o afiamento, foi aplicado o mesmo filtro Gaussiano anterior.  
A aplicação do filtro gerou a imagem central "lMRIBorrado" que é removida da imagem original (subtraída) e então é realizada uma nova normalização que resulta na imagem afiada.  
<p align="center">
<img src = "https://user-images.githubusercontent.com/86500603/209255484-3b2705b4-49d0-469e-b627-7e515abf57c1.png" height = 300>
<img src = "https://user-images.githubusercontent.com/86500603/209255508-b04febe7-0071-443d-8ef4-2508cb3c5ae7.png" height = 300>
<img src = "https://user-images.githubusercontent.com/86500603/209255531-5f088db3-31a4-48d5-b1b6-f171fabe1a3c.png" height = 300>
</p>


Gradiente de uma imagem  
O gradiente de uma imagem é similar a uma derivada direcional, destacando a intensidade de transição entre os pixels em uma direção.  
A direção é definida pelo tipo de máscara/método utilizado. No laboratório analisamos máscaras/operadores de Priwitt, Sobel, Laplaciano, Kirsh, Robinson e Frei-chen.  

Priwitt  
A primeira imagem representa uma imagem de um stent inserido em uma artéria.  
A segunda imagem representa o Priwitt do stent na direção x.  
A terceira imagem representa o Priwitt do stent na direção y.  
A quarta imagem representa o módulo Priwitt, baseado na segunda e terceira imagem.  
<p align="center">
<img src = "https://user-images.githubusercontent.com/86500603/209257187-bf239a77-b0be-4b6b-ad72-0a8cd1b8c91d.png" height = 300>
<img src = "https://user-images.githubusercontent.com/86500603/209257194-a6e1932f-5c36-486b-ba7e-ae879e4b288a.png" height = 300>
<img src = "https://user-images.githubusercontent.com/86500603/209257200-6bbbb47b-62a8-49dc-84ef-7f2b4fd4b523.png" height = 300>
<img src = "https://user-images.githubusercontent.com/86500603/209257392-381f56fb-9d44-4a6b-beac-ff489b4c82d1.png" height = 300>
</p>

Sobel  
A primeira imagem representa o Priwitt do stent na direção x.  
A segunda imagem representa o Priwitt do stent na direção y.  
A terceira imagem representa o módulo Sobel, baseado na primeira e segunda imagem.  
<p align="center">
<img src = "https://user-images.githubusercontent.com/86500603/209257552-486a0129-1bee-4969-882c-74144f5412a3.png" height = 300>
<img src = "https://user-images.githubusercontent.com/86500603/209257565-64d1783d-1297-4747-b135-1d634a8ad47f.png" height = 300>
<img src = "https://user-images.githubusercontent.com/86500603/209257603-7163a75a-b043-4bd8-a3be-e7ab4deb3329.png" height = 300>
</p>
