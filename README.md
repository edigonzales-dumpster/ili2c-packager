# ili2c-packager

jdeps --class-path './*' --multi-release base -recursive --ignore-missing-deps --print-module-deps ili2c.jar


          jpackage --icon icon-compiler-128x128.icns --name ili2c --type ${{matrix.package}} --input libs --main-jar ili2c-${{env.VERSION}}.jar -d output --runtime-image ili2c-jre --app-version ${{env.VERSION}} --java-options -Xmx2g 
