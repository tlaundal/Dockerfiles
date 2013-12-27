# minecraft-spigot
#
# An image for a Spigot Minecraft server

# We build off totokaka/minecraft-base
FROM totokaka/minecraft-base

# We need the spigot jar
ADD http://ci.md-5.net/job/Spigot/lastSuccessfulBuild/artifact/Spigot-Server/target/spigot.jar /minecraft/spigot.jar

# The entry point is just starting the server.
ENTRYPOINT ["java", "-jar", "spigot.jar"]
