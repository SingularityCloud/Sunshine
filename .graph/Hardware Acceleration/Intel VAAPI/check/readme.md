# Check if VAAPI is working
https://docs.lizardbyte.dev/projects/sunshine/en/latest/about/advanced_usage.html#adapter-name

ls /dev/dri/renderD:
'''
sudo apt install vainfo -y

num=128

vainfo --display drm --device /dev/dri/renderD${num} | grep -E "((VAProfileH264High|VAProfileHEVCMain|VAProfileHEVCMain10).*VAEntrypointEncSlice)|Driver version"
'''
—https://github.com/loki-47-6F-64/sunshine/issues/97

# Log:
```Info: Found encoder vaapi: [h264_vaapi]```
