# operator-sdk-devspace
This is a template repository used to run operator-sdk controllers & webhooks in debug mode.

## Quickstart

1. Clone this repo
2. Make the changes you need <br />
	a. If you create an api, uncomment <br />
	```bases:
	#- ../crd
	```
	from the config/default/kustomization.yaml file and <br />
	```
	#- role.yaml
	#- role_binding.yaml
	```
	from the config/rbac/kustomization file.<br />
3. Add to Makefile
   ```NAME ?= <NAME OF THE PROJECT``` (make sure to not include -system, as it will be added)
4. Run ```make devspace```
