#!/bin/bash
set -x
export AWS_ACCESS_KEY_ID=${AWS_ACCESS_KEY_ID}
export AWS_SECRET_ACCESS_KEY=${AWS_SECRET_ACCESS_KEY}
echo "test psw: ${CYPRESS_TEST_PSW}"
#export WORKSPACE="/home/ubuntu/jenkins/workspace/"
export ROOT_U="sudo"

sudo apt-get install libgtk2.0-0 libgtk-3-0 libgbm-dev libnotify-dev libgconf-2-4 libnss3 libxss1 libasound2 libxtst6 xauth xvfb -y
sudo apt-get install chromium-browser -y


echo "############################# npm install ################################"
yarn install

echo "############################# running e2e tests ################################"
bash run_e2e.sh
