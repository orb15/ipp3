# ipp3

Table generators used with [Inspiration pad Pro3](http://www.nbos.com/products/inspiration-pad-pro)

As a hint to myself for later, do the follow steps to set up symlinks to make ipp3 work gracefully with these files:

1. Install IPP3
2. Rename the supplied Generator and Common folders to something else. This hides them from the IPP3 executable
3. Create a Generators and Common folder elsewhere
4. Copy the contents of the Generators and Common folders into their new locations if desired. If you don;t do thios, the default IPP-supplied tables won;t be available
5. Create hard symlinks (see Windows mklink /J option, sigh) in the IPP3 installation directory to the new Generators and Common folders. Test IPP3 - it should see the default table generation if you kept the contents of those folders
6. Drop the 'potato' folder here into the new Generators folder
7. Create a hard symlink from the COmmon folder to the Generators/potato/common folder
8. Rerun IPP3 to make sure all is working as desired
