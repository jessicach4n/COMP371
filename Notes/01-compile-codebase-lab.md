**Inside U:\sandbox\COMP371\Windows\COMP371_all\COMP371_RaytracerBase\code**
1. From here run the CMake application.
2. Select the source as the path above.
3. Select build folder that should be created inside the code folder.
4. Click configure.
5. Click Generate.
6. Open Project with Visual Studio 2019.
7. Build > Build Solution.
8. Right click on raytracer and Set as Startup Project.
9. Run.
10. Debug > raytracer Debug Properties > Debugging > Command Arguments > "../assets/cornell_box_al.json" > apply > OK > Run again.

**For OpenGL**
1. Start a new CMake.
2. Point the source to the code folder of the lab capsule we want.
3. Point the build to the build folder inside the lab capsule folder.
4. Configure.
5. Generate.
6. Open with VS 2019.
7. Build > Build Solution.
8. Right click on capsule02 (or any other capsule used) and Set as Startup Project.
9. Run.

**Docker**
1. In the C: drive, create a folder COMP371
2. Clone https://github.com/ConU-CSSE/COMP371_dockerimage.git
3. Clone https://github.com/tiperiu/COMP371_all.git
4. cd .\COMP371_dockerimage\
5. Open Docker Desktop application
6. Run in the terminal `Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Unrestricted`
7. Run `.\windows\build_docker.ps1`
8. Run `.\windows\interactive_run.ps1 C:\Users\j_chan20\Desktop\COMP371\COMP371_RaytracerBase\code`
9. Mkdir build folder and cd into it.
10. Run `cmake ../`
11. Run `make`
12. Run `./raytracer`

**Docker MacOS**
1. Clone https://github.com/ConU-CSSE/COMP371_dockerimage.git
2. Clone https://github.com/tiperiu/COMP371_all.git
3. cd .\COMP371_dockerimage\
4. Open Docker Desktop application
5. Run `.\linux\build_docker.sh`
6. Run `.\linux\interactive_run.sh /Users/jessica_chan/Documents/GitHub/COMP371_all/COMP371_RaytracerBase/code`
7. cd build
8. Run `cmake ../`
9. Run `make`
10. Run `./raytracer`
11. 10. Run `./raytracer ../assets/cornell_box_al.json`