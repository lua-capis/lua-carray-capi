# Lua Carray C API 
<!-- ---------------------------------------------------------------------------------------- -->

The *Carray C API* makes it possible to handle arrays of primitive numeric C data types in 
[Lua] script code and also in native C code for enhancing module interoperability.

For further documentation see [carray_capi.h](./carray_capi.h).

<!-- ---------------------------------------------------------------------------------------- -->

### Implementation:

   * [carray] - this Lua module provides an implemenation of the *Lua Carray C API*.


### Invocations:
   
   * [mtmsg] - this Lua module invokes the *Lua Carray C API* to make it possible to pass
               arrays of primitive numeric C data types to other threads.

   * [mtstates] - this Lua module invokes the *Lua Carray C API* to make it possible to pass
                  arrays of primitive numeric C data types to other states.

   * [ljack] - audio sender processor objects are able to send audio samples that can be
               passed as *float32* [carray] objects from non realtime threads to a JACK AUDIO 
               OUT port or other realtime audio processor objects, see [ljack.new_audio_sender()], 
               [ljack/example05.lua] and [ljack/example06.lua]

   * [ljack] - midi sender and receiver objects are able to send or receive midi event bytes 
               that can be passed as 8-bit integer [carray] objects from/to non realtime threads 
               to a JACK MIDI port or other realtime audio processor objects, see 
               [ljack.new_midi_sender()], [ljack.new_midi_receiver()] and [ljack/example07.lua].

<!-- ---------------------------------------------------------------------------------------- -->

[Lua]:      https://www.lua.org
[carray]:   https://github.com/osch/lua-carray
[mtmsg]:    https://github.com/osch/lua-mtmsg
[mtstates]: https://github.com/osch/lua-mtstates

[ljack]:                     https://github.com/osch/lua-ljack
[ljack/example05.lua]:       https://github.com/osch/lua-ljack/blob/master/examples/example05.lua
[ljack/example06.lua]:       https://github.com/osch/lua-ljack/blob/master/examples/example06.lua
[ljack/example07.lua]:       https://github.com/osch/lua-ljack/blob/master/examples/example07.lua
[ljack.new_audio_sender()]:  https://github.com/osch/lua-ljack/blob/master/doc/README.md#ljack_new_audio_sender
[ljack.new_midi_sender()]:  https://github.com/osch/lua-ljack/blob/master/doc/README.md#ljack_new_midi_sender
[ljack.new_midi_receiver()]:  https://github.com/osch/lua-ljack/blob/master/doc/README.md#ljack_new_midi_receiver

<!-- ---------------------------------------------------------------------------------------- -->

## License 

This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or distribute this
software, either in source code form or as a compiled binary, for any purpose,
commercial or non-commercial, and by any means.

<!-- ---------------------------------------------------------------------------------------- -->
