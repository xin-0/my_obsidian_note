use existed roslaunch file and set the parameter in that file 
```
<include file="$(find pkg_name)/pkg/.launch">
	<arg name="arg1"     value="val"/>
</include>
```