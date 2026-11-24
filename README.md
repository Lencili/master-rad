# Master rad — PINN i inferenca (MATF, astroinformatika)

Priprema za master rad: statističke osnove fitovanja modela, MCMC, Flow Matching i physics-informed neuronske mreže (PINN).

## Struktura

| Folder | Sadržaj |
|---|---|
| `00_osnove_bajesovska_inferenca/Hogg_fitovanje` | Vežbe iz Hogg, Bovy, Lang (2010), *Data analysis recipes: Fitting a model to data* — najmanji kvadrati, mešavinski model za autlajere, ručni MCMC, bootstrap/jackknife, greške po x i y, intrinzično rasipanje |
| `00_osnove_bajesovska_inferenca/emcee_MCMC` | Primeri iz dokumentacije biblioteke emcee — quickstart, fit linije sa potcenjenim greškama, vreme autokorelacije, čuvanje lanca, paralelizacija, potezi |
| `01_flow_matching` | Flow Matching (FMPE) za problem linearne regresije, poređenje sa tačnim posteriorom i provera kalibracije |
| `02_PINNs` | PINN za prigušeni harmonijski oscilator: direktni problem i inverzni problem (određivanje nepoznatog μ), uticaj težine λ, otkrivanje jednačine; prati ETH DLSC 2023, predavanje „PINNs – Applications“ |

## Pokretanje

```
pip install numpy scipy matplotlib torch emcee corner h5py tqdm
```

Notebook-i su već pokrenuti i sadrže rezultate i grafike.

## Izvori

- Hogg, Bovy, Lang (2010), [arXiv:1008.4686](https://arxiv.org/abs/1008.4686)
- emcee dokumentacija: https://emcee.readthedocs.io/en/stable/ ; Foreman-Mackey i sar. (2013), [arXiv:1202.3665](https://arxiv.org/abs/1202.3665)
- Lipman i sar. (2023), *Flow Matching for Generative Modeling*, [arXiv:2210.02747](https://arxiv.org/abs/2210.02747)
- Dax i sar. (2023), *Flow Matching for Scalable Simulation-Based Inference*, [arXiv:2305.17161](https://arxiv.org/abs/2305.17161)
- ETH Zürich, *Deep Learning in Scientific Computing 2023*: https://camlab.ethz.ch/teaching/deep-learning-in-scientific-computing-2023.html ; kod: https://github.com/benmoseley/DLSC-2023
- Raissi, Perdikaris, Karniadakis (2019), *Physics-informed neural networks*, J. Comput. Phys.
