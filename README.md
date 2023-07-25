# k8s-jenkins

## project usage
It can be used with open im server and can be copied to the project directory separately

## directory structure
```
.
├── LICENSE
├── Makefile // use in open im server. the content has been adjusted
├── README.md 
├── component // component configuration. like mysql, kafka
├── dockerfile // server dockerfile configuration
├── jenkinsfiles // jenkins template
└── k8sdeployment_dev // server k8s deploy template
```

## use in different situations

> please prepare two things
```shell
1.k8s namespace has created
2.docker register project has created
```

### use jenkins

1. create view
2. copy the files in the jenkinsfiles as the configuration file for the pipeline
3. fill some environment parameters in file
4. choice specific branch and project, and click build