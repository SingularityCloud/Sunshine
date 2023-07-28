# Check if VAAPI is working
https://github.com/loki-47-6F-64/sunshine/issues/97

'''
sudo apt install vainfo -y

num=128

vainfo --display drm --device /dev/dri/renderD${num} | grep -E "((VAProfileH264High|VAProfileHEVCMain|VAProfileHEVCMain10).*VAEntrypointEncSlice)|Driver version"
'''
