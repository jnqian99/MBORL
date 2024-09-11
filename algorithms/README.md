## Usage

cd ORL_optimizer  #replace with the parent folder containing MBORL

To evaluate with myenv simulator and the gym environment with Rebrac:

python3 MBORL/algorithms/rebrac_main.py --config MBORL/config/hopper/rebrac_hopper_medium_v2.yaml

## FILES

- rebrac_main.py

The main file to train Rebrac

- rebrac_model.py

the model architecture of the components

- rebrac_update.py

update actor and critic moduels based on RebRac

- rebrac_util.py

config files and get data loader and D4RL

- rebrac_eval.py

evaluate gym - evalute simulated env - get transition from simulated env for data augmentation

- rebrac_plot_sim.py

evalute and plot the states, rewards, vae of my simulator model vs. Gym with actions based on my simulator using rebrac policy

- rebrac_plot_gym.py

similar to rebrac_plot_sim.py but uses actions based on states from Gym
