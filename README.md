# DPML
Multi-Objective Optimization with Dynamic Programming-Based Meta-Reinforcement Learning 
# Dependencies
Python>=3.6 <br>
NumPy <br>
PyTorch>=1.4 <br>
# Meta-Learning
For training meta-model on MOTSP-20 instances: <br>
python run.py --graph_size 20 --CUDA_VISIBLE_ID "0" --is_train --meta_iterations 10000
For training meta-model on MOTSP-50 instances: <br>
python run.py --graph_size 50 --CUDA_VISIBLE_ID "0" --is_train --meta_iterations 5000
You can initialize or resume a run using a pretrained meta-model by using the --load_path option, e.g.: <br>
python run.py --graph_size 50 --is_load --load_path "meta-model-MOTSP50.pt" --CUDA_VISIBLE_ID "0" --is_train --meta_iterations 10000 --start_meta_iteration 5000
