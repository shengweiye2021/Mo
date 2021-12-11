

## Datasets

In the dataset folder, we provide all three processed datasets used in MolTrans: BindingDB, DAVIS, and BIOSNAP. In BIOSNAP folder, there is full dataset for the main experiment, and also missing data experiment (70%, 80%, 90%, 95%) and unseen drug and unseen protein datasets.

## Run

We provide an example jupyter notebook in the repository. Although it runs for 100 epochs, we find 50 epochs is way enough and all the results in paper are run by 50 epochs. 

You can also directly run `python train.py --task ${task_name}` to run the experiments. `${task_name}` could either be `biosnap`,`bindingdb` , and `davis`. For the BindingDB and DAVIS, please refer this [Page](https://zitniklab.hms.harvard.edu/TDC/multi_pred_tasks/dti/) for more details.

Will add more codes and tests in the next couple of weeks. But this should be enough to try on MolTrans.


主要是在train.py里修改

单机单线程多gpu可以运行；

问题和需求：
无法使用单机多线程多卡运行程序。


[数据集](https://mail.google.com/mail/u/0?ui=2&ik=01af9d1bc1&attid=0.1&permmsgid=msg-a:r2731998933004499938&th=17da4c7299612322&view=att&disp=inline&realattid=f_kx0hsxd00)
