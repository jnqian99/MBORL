## Usage

cd ORL_optimizer #replace with the parent folder containing MBORL

to train using offline data:

python3 MBORL/simulators/env_train_offline.py --config MBORL/config/hopper/env_hopper_medium_v2.yaml

to train vae:

python3 MBORL/simulators/env_train_vae.py --config MBORL/config/hopper/env_hopper_medium_v2.yaml

to plot states and rewards for autoregressive, non-autoregressive vs true values, and caculate R^2 values based on test data:

python3 MBORL/simulators/env_plot.py --config MBORL/config/hopper/env_hopper_medium_v2.yaml

## Files

- env_model.py

contains models and MyEnv

- env_util.py

common utility classes for config parsing and getting sample batch

- env_train_offline.py

training for environment using offline d4rl data, use env_... . yaml file both AR and NAR

- env_train_vae.py

train VAE from the model in env_mod and save checkpt in config folder

- env_plot.py

plotting and returns R2 data, predicted reward and few state AR vs NAR
