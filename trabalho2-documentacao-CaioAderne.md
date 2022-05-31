# Trabalho 2: Integração de habilidades - 2022/1
**Disciplina: Redes de Computadores**

**Curso: Engenharia de Computação**

**Caio Gabriel Aderne de Melo/RA: 1636820**


## Tarefa 1:  Sub-Redes
| Sub- Rede |             IPv6 - Sub-Rede            |  IPv4 - Sub-Rede  |  IPv4 - Máscara   | IPv4 - Broadcast  |    
|:---------:|:--------------------------------------:|:-----------------:|:-----------------:|:-----------------:|
| Matriz    | 2001:DB8:ACAD:1400::/64 | 200.200.20.0   | 255.255.255.192 | 200.200.N.63  |
| Filial 1  | 2001:DB8:ACAD:1401::/64 | 200.200.20.64  | 255.255.255.224 | 200.200.N.95  |
| Filial 2  | 2001:DB8:ACAD:1402::/64 | 200.200.20.96  | 255.255.255.224 | 200.200.N.127 |
| Filial 3  | 2001:DB8:ACAD:1403::/64 | 200.200.20.128 | 255.255.255.224 | 200.200.N.159 |
| Filial 4  | 2001:DB8:ACAD:1404::/64 | 200.200.20.160 | 255.255.255.224 | 200.200.N.192 |
| Filial 5  | 2001:DB8:ACAD:1405::/64 | 200.200.20.192 | 255.255.255.224 | 200.200.N.223 |
| pb-vit    | 2001:DB8:ACAD:14FF::0:0/112 | 200.200.20.224 | 255.255.255.252 | 200.200.N.227 |
| vit-fb    | 2001:DB8:ACAD:14FF::1:0/112 | 200.200.20.228 | 255.255.255.252 | 200.200.N.231 |
| fb-ita    | 2001:DB8:ACAD:14FF::2:0/112 | 200.200.20.232 | 255.255.255.252 | 200.200.N.235 |
| ita-pb    | 2001:DB8:ACAD:14FF::3:0/112 | 200.200.20.236 | 255.255.255.252 | 200.200.N.239 |
| cv-ita    | 2001:DB8:ACAD:14FF::4:0/112  | 200.200.20.240 | 255.255.255.252 | 200.200.N.243 |


## Tarefa 2: Endereçamento de Dispositivos
| Dispositivo           | Interface | IPv4 | IPv4 - Máscara | IPv4 - Gateway | IPv6/Prefixo | IPv6 - Gateway |
|-----------------------|-----------|------|----------------|----------------|--------------|----------------|
| PC1 | NIC    |   200.200.20.3   |      255.255.255.192     |      200.200.20.1       |       2001:db8:acad:1400::3/64       |        FE80::1        |
| PC2 | NIC    |   200.200.20.4 |	255.255.255.192 |	200.200.20.1 |	2001:db8:acad:1400::4/64 |	FE80::1 |
| PC3 | NIC    |   200.200.20.67 |	255.255.255.224 |	200.200.20.65 | 2001:db8:acad:1401::3/64 |	FE80::1  |
| PC4 | NIC    |    200.200.20.68 |	255.255.255.224 |	200.200.20.65 | 2001:db8:acad:1401::4/64 |	FE80::1 |
| PC5 | NIC    |   200.200.20.131   |	255.255.255.224   |	200.200.20.129   | 2001:db8:acad:1402::3/64   |	FE80::1   |
| PC6 | NIC    | 200.200.20.131 |	255.255.255.224 |	200.200.20.129 | 2001:db8:acad:1402::4/64 |	FE80::1     |
| Switch-Matriz | SVI    |  200.200.20.2|	255.255.255.192|	200.200.20.2          |
| Switch-Filial1 | SVI    |   200.200.20.66|	255.255.255.224|	200.200.20.66       |
| Switch-Filial2 | SVI    |  200.200.20.130|	255.255.255.224|	200.200.20.130     |
| Roteador-Pato Branco  | Fa0/0 |      |                |                |              |                |
| Roteador-Pato Branco  | Se0/0/0 |      |                |                |              |                |
| Roteador-Pato Branco  | Se0/0/1 |      |                |                |              |                |
| Roteador-Fco. Beltrão | Fa0/0     |      |                |                |              |                |
| Roteador-Fco. Beltrão | Se0/0/0        |                |                |              |                |
| Roteador-Fco. Beltrão | Se0/0/1 |      |                |                |              |                |
| Roteador-Vitorino     | Se0/0/0 |      |                |                |              |                |
| Roteador-Vitorino     | Se0/0/1 |      |                |                |              |                |
| Roteador-Itapejara    | Se0/0/0 |      |                |                |              |                |
| Roteador-Itapejara    | Se0/0/1 |      |                |                |              |                |
| Roteador-Itapejara    | Fa0/1   |      |                |                |              |                |
| Roteador-Coronel      | Fa0/0   |      |                |                |              |                |
| Roteador-Coronel      | Se0/0/1 |      |                |                |              |                |
| Roteador-Coronel      | Fa0/1  |      |                |                |              |                |

## Tarefa 3: Tabela de Roteamento
### Roteador Pato Branco
#### IPv4
| Rede de Destino | Máscara | Next Hop | Interface de Saída |
|-----------------|---------|----------|--------------------|
|                 |         |          |                    |
|                 |         |          |                    |
|                 |         |          |                    |
#### IPv6
| Rede de Destino/Prefixo | Next Hop | Interface de Saída |
|-----------------|----------|--------------------|
|                 |          |                    |
|                 |          |                    |
|                 |          |                    |


## Topologia - Packet Tracer
- [ ] ![Trabalho2-Topologia-NomeAluno](trabalho2-topologia-NomeAluno.pkt)


## Arquivos de Configuração dos Dispositivos Intermediários (roteadores e switches)
- [ ] ![Roteador Pato Branco](r-pb-nnn.pkt)
- [ ] ![Roteador Francisco Beltrão](r-fb-nnn.pkt)
- [ ] ![Roteador Vitorino](r-vit-nnn.pkt)
- [ ] ![Roteador Itapejara D'Oeste](r-ita-nnn.pkt)
- [ ] ![Roteador Coronel Vivida](r-cv-nnn.pkt)
- [ ] ![Switch Pato Branco](sw-pb-nnn.pkt)
- [ ] ![Switch Francisco Beltrão](sw-fb-nnn.pkt)
- [ ] ![Switch Coronel Vivida](sw-cv-nnn.pkt)


