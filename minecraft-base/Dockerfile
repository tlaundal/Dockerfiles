# minecraft-base
#
# This is inteded as a parent for minecraft servers.
# The only difference between this and arch-java is that we create an user
# called minecraft which the minecraft server can run from.

# We build off the arch-java package, which is the minimal arch install with a 
# headless java jre.
FROM arch-java
MAINTAINER totokaka <mail@totokaka.io>

# Set up the user minecraft with /minecraft as home directory.
RUN useradd -s /bin/bash -d /minecraft -m minecraft

# _All_ Minecraft related stuff run on port 25565, even if another port is used
# the port can be forwarded by Docker
EXPOSE 25565

# From now on, everything can be run from the minecraft user
USER minecraft