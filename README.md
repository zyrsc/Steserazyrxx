Traceback (most recent call last):
  File "/home/container/.local/lib/python3.14/site-packages/discord/ext/commands/converter.py", line 1359, in _actual_conversion
    return converter(argument)
ValueError: invalid literal for int() with base 10: 'Haaland'
The above exception was the direct cause of the following exception:
Traceback (most recent call last):
  File "/home/container/.local/lib/python3.14/site-packages/discord/ext/commands/bot.py", line 1376, in invoke
    await ctx.command.invoke(ctx)
  File "/home/container/.local/lib/python3.14/site-packages/discord/ext/commands/core.py", line 1056, in invoke
    await self.prepare(ctx)
  File "/home/container/.local/lib/python3.14/site-packages/discord/ext/commands/core.py", line 973, in prepare
    await self._parse_arguments(ctx)
  File "/home/container/.local/lib/python3.14/site-packages/discord/ext/commands/core.py", line 880, in _parse_arguments
    transformed = await self.transform(ctx, param, attachments)
                  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/container/.local/lib/python3.14/site-packages/discord/ext/commands/core.py", line 750, in transform
    return await run_converters(ctx, converter, argument, param)  # type: ignore
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/container/.local/lib/python3.14/site-packages/discord/ext/commands/converter.py", line 1466, in run_converters
    return await _actual_conversion(ctx, converter, argument, param)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/container/.local/lib/python3.14/site-packages/discord/ext/commands/converter.py", line 1368, in _actual_conversion
    raise BadArgument(f'Converting to "{name}" failed for parameter "{param.name}".') from exc
discord.ext.commands.errors.BadArgument: Converting to "int" failed for parameter "miktar".
