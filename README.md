# GODOT-Basic-Loading-Screen-Utility

This utility consists of a scene with progress bar and an image animation and a script that manages scene preloading and shader precompilation.

To do this, the following parameters must be configured:

* _progress_speed : float -> Indicates the speed at which the progress bar completes to indicate the progress of this process. Ultimately, the preload time will determine the elapsed time. With this parameter you can slow down the animation of the preloading and precompilation process.

* _scene_path : String -> Indicates the scene that will be loaded once the preload and precompilation process is complete.

* _scene_paths : Array[String] -> Indicates the list of scenes to be preloaded.

* _materials : Array[String] -> Indicates the list of materials to be precompiled.

  If an autoload mandatorily called GameInstance is created, it may contain the declaration of the variables _scene_path, _scene_paths, and _materials, in which case these will be taken into account instead of those defined in the utility itself. ( _progress_speed can only be configured in the utility)

Note that if you want to reuse the utility to transition between different levels, this is the most convenient way, rather than duplicating the utility, renaming it, and using different copies for each transition.

If the utility is only needed for an initial preload and precompile screen, the most convenient way would be to configure the variables in the utility.

This utility has been tested in https://jocarpe.itch.io/third-person-character-demo

This is a demo in continuous development to test all the components developed and in the process of future development.

It also adds the ability to change characters and view resource consumption via a plugin.

A detailed explanation of how the demo works is available on the itch.io page indicated.

Feel free to check it out in either of its two versions, Windows or Linux.
