# :dark_sunglasses: [Classy](https://github.com/sunglasses-ai/classy) Template

Welcome! If you're landing here, it's probably because you want to try out our library, [classy](https://github.com/sunglasses-ai/classy).

As you might have read from our [documentation](https://sunglasses-ai.github.io/classy/docs/intro), `classy` comes with a bunch of ready-to-use tools and tasks.
But, for more particular settings (as yours is, probably!), we have developed this template that we have specifically built to seamlessly integrate with `classy`.

In case you didn't, check out [`classy`'s preconfigured tasks](https://sunglasses-ai.github.io/classy/docs/reference-manual/tasks-and-formats/) to make sure it doesn't cover your use case already! We cover quite a few tasks, including the most common ones! :fire: 

If we did not match your needs (...sorry!), click on [use this template](https://github.com/sunglasses-ai/classy-template/generate) at the top of this page to start.

## :computer: Creating your environment

The best way to start things off is by creating the environment. Once you have cloned your new repository locally, just type `bash setup.sh` and follow the setup script.
It will automatically install all requirements listed inside `requirements.txt` along with `classy` (and its autocomplete).


And... **You're all set**! Yes, it's that easy.

## :question: What can/should I do?

Well, there are a few (basic) things that you might be interested in doing:

- Creating a custom model [(link)](https://sunglasses-ai.github.io/classy/docs/getting-started/overriding-code/custom-model)
- Creating a custom dataset [(link)](https://sunglasses-ai.github.io/classy/docs/advanced/custom-dataset/)
- Creating a custom data reader [(link)](https://sunglasses-ai.github.io/classy/docs/getting-started/overriding-code/custom-data-form/)

#### :scroll: Examples

Additionally, that we have an ever-growing [repository of examples](https://github.com/sunglasses-ai/classy-examples) available that touch most parts of `classy`'s structure.

## :robot: How does `classy` integrate with the template?

Great question! 

For starters, `classy` will automatically discover any configuration files you add under `configurations/` and will also automatically discover any :snake: Python file defined under `src/`!

This way, you can easily change the model you train from the `classy` CLI by doing

```diff
classy train <task> <dataset> -n <exp-name> \
+      -c model._target_=src.model.MyCustomClassyModel
```

## :sos: Help / get in touch

Finally, if you need help, want to report a bug, or just want to get in touch, [open an issue](https://github.com/sunglasses-ai/classy/issues/new) on the main `classy` repository or join us on [Slack](https://sunglasses-ai.slack.com)!
