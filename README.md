# R3-MolGAN

Baseline model: [EDM](https://github.com/ehoogeboom/e3_diffusion_for_molecules), trained on [nablaDFT](https://github.com/AIRI-Institute/nablaDFT/).
To reproduce our results:

```shell
git clone https://github.com/ehoogeboom/e3_diffusion_for_molecules.git
wget 'https://a002dlils-kadurin-nabladft.obs.ru-moscow-1.hc.sbercloud.ru/data/nablaDFTv2/energy_databases/train_100k_v2_formation_energy_w_forces.db'
cp scripts/diff_nabla.py e3_diffusion_for_molecules/
cp scripts/sascorer.py e3_diffusion_for_molecules/
cd e3_diffusion_for_molecules
pip install .
python diff_nabla.py
```
