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

   * [auproc] - audio sender processor objects are able to send audio samples that can be
                passed as *float32* [carray] objects from non realtime threads to an 
                [auproc-capi] connector, see [auproc.new_audio_sender()], 
                [ljack/example05.lua] and [ljack/example06.lua]

   * [auproc] - midi sender and receiver objects are able to send or receive midi event bytes 
                that can be passed as 8-bit integer [carray] objects from/to non realtime threads 
                to an [auproc-capi] connector, see [auproc.new_midi_sender()], 
                [auproc.new_midi_receiver()], [ljack/example03.lua]
                and [ljack/example04.lua].

   * [lfft]   - Fast Fourier Transformation operates on arrays of *float* or *double* element 
                type.

<!-- ---------------------------------------------------------------------------------------- -->

[Lua]:      https://www.lua.org
[carray]:   https://github.com/osch/lua-carray
[mtmsg]:    https://github.com/osch/lua-mtmsg
[mtstates]: https://github.com/osch/lua-mtstates
[lfft]:     https://github.com/osch/lua-lfft

[ljack]:                     https://github.com/osch/lua-ljack
[ljack/example03.lua]:       https://github.com/osch/lua-ljack/blob/master/examples/example03.lua
[ljack/example04.lua]:       https://github.com/osch/lua-ljack/blob/master/examples/example04.lua
[ljack/example05.lua]:       https://github.com/osch/lua-ljack/blob/master/examples/example05.lua
[ljack/example06.lua]:       https://github.com/osch/lua-ljack/blob/master/examples/example06.lua
[ljack/example07.lua]:       https://github.com/osch/lua-ljack/blob/master/examples/example07.lua

[auproc]:                    https://github.com/osch/lua-auproc
[auproc-capi]:               https://github.com/lua-capis/lua-auproc-capi

[auproc.new_audio_sender()]:  https://github.com/osch/lua-auproc/blob/master/doc/README.md#auproc_new_audio_sender
[auproc.new_midi_sender()]:   https://github.com/osch/lua-auproc/blob/master/doc/README.md#auproc_new_midi_sender
[auproc.new_midi_receiver()]: https://github.com/osch/lua-auproc/blob/master/doc/README.md#auproc_new_midi_receiver

<!-- ---------------------------------------------------------------------------------------- -->

## License 

This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or distribute this
software, either in source code form or as a compiled binary, for any purpose,
commercial or non-commercial, and by any means.

<!-- ---------------------------------------------------------------------------------------- -->
