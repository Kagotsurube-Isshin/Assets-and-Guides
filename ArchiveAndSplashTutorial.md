# Archive and Splash Images Modding How-To-Save Tutorial

### This is *not* a tutorial on how to mod these, rather how to save them, as they need a specific type of .dds formatting to show properly. For how to start modding these, [click here.](https://github.com/SilentNightSound/GI-Model-Importer/blob/main/Guides/TextureModdingTutorial.md)

Normal textures save in the .dds subtypes of BC7 Linear/sRGB DX11+, with "Generate Mip Maps" ticked. *However* these are NOT the formats archive icons, icon miniatures, and splash art should be saved as, as it overly compresses them and generates artifacts.

_This was written with paint.net in mind, and I cannot answer for Photoshop saving as I find it unreliable for this case usage. If you use PS, save the image as PNG or TGA, then re-save from paint.net._

### The ideal format for these files is R8G8B8A8 (Linear, A8B8G8R8) WITH MIP MAPS OFF.
### Flatten the image before saving, as multiple layers are more likely to generate artifacts.

## Archive icons

![image](https://user-images.githubusercontent.com/131506884/235824355-e9a0b2de-ba45-4eb2-9ebb-735448668925.png)![image](https://user-images.githubusercontent.com/131506884/235824495-61d21717-77c2-44cf-a048-8c6eefc44ad6.png)![image](https://user-images.githubusercontent.com/131506884/235824546-8b240391-213d-4646-a9c2-67993c091256.png)

![image](https://user-images.githubusercontent.com/131506884/235815813-9365e2d7-abdd-449e-a9ce-c17b9421a83d.png)![image](https://user-images.githubusercontent.com/131506884/235815913-ac7196d8-3eb4-4648-b038-654b36a0f320.png)![image](https://user-images.githubusercontent.com/131506884/235823011-4a0b9e3f-198f-4f01-b6ac-917294034bb0.png)

- Unmodded
- Saved with Mip Maps
- Saved without Mip Maps




## Some large examples in splash edits
![image](https://user-images.githubusercontent.com/131506884/235823281-1ae3b21d-e1bc-4b92-b771-fe45d3b56097.png)

- Unmodded

![image](https://user-images.githubusercontent.com/131506884/235823486-98993b7f-cae5-4172-a7a2-e346126138d4.png)

- Saved as BC7 Linear DX11+ with Mip Maps

![image](https://user-images.githubusercontent.com/131506884/235823648-041ff228-a314-48e2-8786-be214128d9bd.png)

- Saved as BC7 Linear DX11+ without Mip Maps (yes, they look the about the same)

![image](https://user-images.githubusercontent.com/131506884/235823967-a47e634f-3a61-46a2-93b2-c90fa357b2f2.png)

- Saved as R8G8B8A8 (Linear, A8B8G8R8) without Mip Maps


RA8888 without Mip Maps is the only format that consistently prints without artifacts and compressing out of the rest (spent too much time testing all of them).
Other types of 8888 also seem to look alright, but I've found this particular set produces the least edge noise, if at all.
The files do end up pretty big though, splash art is usually around 8MB on this format.
