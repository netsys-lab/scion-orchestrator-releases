# scion-orchestrator-releases
Stores releases of the scion-orchestrator project for the SCION Education, Research and Academic Network SCIERA of all known ASes that run our bootstrapping servers.

## Get Started
At first navigate to [Releases](https://github.com/netsys-lab/scion-orchestrator-releases/releases) and search for the SCION AS that you want to bootstrap in. Then open the release and search for the archive that is targeted for your operating system. Download the archive on the host that you want to run SCION on. Now extract the archive somewhere on your machine. Next, follow the OS specific instructions:

### Linux/MacOS
To test the SCION endhost stack, move into the extracted folder. Then run `sudo ./scion-orchestrator run`. It should start up and not display any errors.

You can then test if you can reach the SCION network via `./bin/scion showpaths 71-20965`.

To install SCION system wide, run the following command `sudo ./scion-orchestrator install`. This will install SCION as a system service and copy the SCION binaries to the correct folders, you can now run SCION commands without having the `./bin` directory in them: `scion showpaths 71-20965`.

### Windows 
To run the SCION endhost stack, move into the extracted folder. Open a `cmd` terminal with Administrator rights in the extracted folder. Then run `scion-orchestrator.exe run`. It should start up and not display any errors.

To test SCION connectivity, move into `./bin` and run `scion.exe showpaths 71-20965`.

**Note:** With the current release we don't support installing SCION as a system service yet. Stay tuned, this will follow soon!

## Contact us
If you encounter any issues or are interested in setting up your own bootstrap server, please contact us via an issue here or via mail `marten.gartner@ovgu.de`.
