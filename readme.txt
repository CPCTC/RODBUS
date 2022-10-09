# RODBUS
## Reasonably Okay Default BUild Script

RODBUS is a Ccache wrapper that provides higher-level build system features, like automatic source detection, scoped compiler flag configuration, and parallel builds. It still works without Ccache, but at greatly reduced speed.

RODBUS itself is competely stateless between invocations, making Ccache do all the real work. For example, even on a cache hit, you will still see compiler warnings for every file. For this reason, I prefer RODBUS over more conventional build systems.

RODBUS is pretty easy to set up: copy the tiny little bash script into your repo. If you need something specific, you can modify the script as appropriate.
