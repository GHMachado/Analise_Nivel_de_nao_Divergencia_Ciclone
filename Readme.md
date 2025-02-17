# 📈 Análise do nível de não divergência (NND) de um ciclone 🌀

<img height='650px' src="Figure 2024-01-20 114305.png" alt="plot de analise">

> Neste repositório encontram-se códigos para fazer uma análise do NDD de um ciclone tropical/subtropical a partir dos dados de Omega e Divergência da reanálise ERA5.


## 💬 Recomendações

É importante criar um novo ambiente virtual para evitar bugs e erros nos scripts, sendo também considerada uma boa prática de programação. Para criar um ambiente virtual pelo pacote [Anaconda](https://www.anaconda.com/download), siga o tutorial abaixo:

### Windows

### 1° Passo:

Faça o download instalação do pacote Anaconda, siga esse [vídeo](https://www.youtube.com/watch?v=lC8_WhLJWMc) como um guia.

Após a instalação, abra o Anaconda prompt e insira o comando:  

> Desconsidere as "" em todos os comandos.

```
conda create -n "Nome do ambiente" spyder
```
> Se preferir instalar o pacote anaconda completo nesse ambiente, apenas adicione anaconda no final ao invés de spyder e desconsidere o passo de instalação das bibliotecas.

Isso irá criar um novo ambiente virtual que será utilizado para rodar os scripts.

### 2° Passo:

Para ativá-lo, caso tenho fechado o prompt, abra novamente, e digite:
```
conda activate "Nome do ambiente"
```
> Para ter certeza que você entrou no seu ambiente virtual, onde estaria escrito "base" no prompt, agora está escrito o "Nome do ambiente"

### 3° Passo: (Desconsidere se você instalou toda a biblioteca Anaconda no ambiente virtual)

Feito isso, vamos instalar as bibliotecas que iremos utilizar. Utilize o comando:

```
conda install -c conda-forge matplotlib xarray numpy pandas
```

#### Após isso, seu ambiente virtual estará pronto para rodar os códigos. 

## 💻 Utilizando os scripts

Os scripts estão divididos de 3 formas:

1. [Divergencia.py](https://github.com/GHMachado/Plots_para_Omega_e_divergencia_ERA5/blob/main/Divergencia.py) - Plota apenas o perfil vertical de divergência
2. [Omega.py](https://github.com/GHMachado/Plots_para_Omega_e_divergencia_ERA5/blob/main/Omega.py) - Plota apenas o perfil vercial do Omega
3. [Omega_divergencia.py](https://github.com/GHMachado/Plots_para_Omega_e_divergencia_ERA5/blob/main/Omega_divergencia.py) - Plota os dois perfis verticais, lado a lado.

Os scripts são utilizados para fazer uma análise do NDD de um ponto com Lat/Lon específico, sendo necessário carregar um arquivo .csv com os pontos de interesse a serem estudados. \
\
Também é necessário carregar um arquivo Netcdf (.nc de preferência, não foi testado com arquivos .grib) com dados de "Vertical Velocity" e "Divergence" retirados da [Reanálise ERA5](https://cds.climate.copernicus.eu/datasets/reanalysis-era5-pressure-levels?tab=download). Escolha os níveis de pressão de interesse para fazer esse estudo. \
\
Essas são as únicas exigências que os scripts possuem para funcionar corretamente, personalize o gráfico gerado a sua necessidade e gosto.

## 📖 Estudo de caso

Esses scripts foram utilizados para um estudo sobre o NDD do [Furacão Ophelia (2017)](https://www.nhc.noaa.gov/data/tcr/AL172017_Ophelia.pdf) para o trabalho final da disciplina de Sinótica I, que posteriormente foi apresentado na [CPAM 2024](https://cpam2024.com/).

O estudo foi desenvolvido por [Gabriel Machado](https://github.com/GHMachado), [Ronaldo Albuquerque](https://github.com/albqrqe) e Ana Luiza Perry, com orientação da Prof. Ana Cristina Palmeira.

Qualquer dúvida sobre este trabalho, entre em contato.


