# How to make an all-in-one workstation at home

Here's my own experience and personal flavor on budget components selection. Just take as a record.

## some hints

* pratice calculation by yourself
* avoid weired stuff

## prerequisite

**system**
* Debian 12 bookworm / Ubuntu 24.04 LTS
while both got `apt-get`, i'd prefer `debian` more as `ubuntu-snap` is very complicate for me to cope with

**container**
* docker-ce 
de-facto standard for container deployment

**storage**
* openzfs, as it is **simple enough** when you use without edge-conditions

**software-stack**
* jupyterlab / jupyterhub
for code-integrating and EAFP(Easier to Ask for Forgiveness than Permission) style working

* rstudio-server
for data-analysis purpose, which is a commercial product from [Posit](https://posit.co/downloads/)

* samba
for file-sharing, made by the legendary programmer, [Andrew Tridgell](https://en.wikipedia.org/wiki/Andrew_Tridgell), who is also the author of file sync/share tools
    * [samba](https://en.wikipedia.org/wiki/Samba_(software))
    * [Rsync](https://en.wikipedia.org/wiki/Rsync)
    * [Rclone](https://rclone.org/)

* vLLM local-AI-API + OpenWebUI frontend
for LLM-assist modern-era work
    * [vllm-project/vllm](https://github.com/vllm-project/vllm/releases)
    * [open-webui/open-webui](https://github.com/open-webui/open-webui)