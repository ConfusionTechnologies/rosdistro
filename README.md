# ConfusionTechnologies' ROS Package Index

To browse the ROS Main Index, go to <https://index.ros.org/> (note: `pip` packages are considered system dependencies).

This fork of [`rosdistro`](https://github.com/ros/rosdistro) is ConfusionTechnologies' 3rd-party ROS Package Index. It faciliates testing packages we have not published by allowing us to use the normal `rosdep` method instead of workarounds to install them. It also allows adding [rosdep rules](http://docs.ros.org/en/independent/api/rosdep/html/contributing_rules.html), which allows using `pip` packages not present in the main index yet (until pull requests to add said rosdep rules to the main index are accepted).

Take note of the below two branches, which are also **write-protected**:

- `main`: ConfusionTechnologies' ROS Package Index
- `upstream`: Mirror of the upstream ROS Main Package Index

See <https://github.com/ros/rosdistro#readme> for the original README.

## Using

See <http://docs.ros.org/en/independent/api/rosdep/html/contributing_rules.html#point-your-sources-list-d-at-your-forked-repository>. Note to put the correct branch.

## Contributing

Always name your branch `<username>/<description>`. For example, `interpause/add-py3-aiortc-pip`.

### Adding `pip` Dependencies

Branches should be based on `upstream`, **not `main`**! This is to facilitate submitting such `pip` dependencies to the main index. See <http://docs.ros.org/en/independent/api/rosdep/html/contributing_rules.html>.

### Adding Packages

TBD

### Publishing Packages

Good luck. The foundational packages don't follow their [naming guidelines](https://www.ros.org/reps/rep-0144.html). Otherwise, refer to ROS' [contribution guide](https://github.com/ros/rosdistro/blob/master/CONTRIBUTING.md).
