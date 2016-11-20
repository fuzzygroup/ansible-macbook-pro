# ansible-macbook-pro

This is a git repo designed to configure a 2016 Macbook Pro for the needs of a Ruby / OSS developer.  

Here's the [blog post describing it]().

Here's the output of the Ansible playbook command, warts and all:

    Js-MacBook-Pro:ansible-macbook-pro sjohnson$ ansible-playbook -i inventories/hosts playbook_macbook_pro.yml

    PLAY [all] *********************************************************************

    TASK [setup] *******************************************************************
    ok: [0.0.0.0]

    TASK [machine_setup : Ensure the user SSH directory exists] ********************
    ok: [0.0.0.0]

    TASK [machine_setup : Ensure user known hosts file exists] *********************
    ok: [0.0.0.0]

    TASK [machine_setup : Ensure the Ansible downloads directory exists] ***********
    ok: [0.0.0.0]

    TASK [machine_setup : Ensure user known hosts file exists] *********************
    ok: [0.0.0.0]

    TASK [install_browsers : install_google_chrome] ********************************
    ok: [0.0.0.0]

    TASK [install_browsers : chrome-devtools] **************************************
    ok: [0.0.0.0]

    TASK [install_browsers : chromium] *********************************************
    ok: [0.0.0.0]

    TASK [install_browsers : firefox] **********************************************
    ok: [0.0.0.0]

    TASK [install_browsers : vivaldi] **********************************************
    ok: [0.0.0.0]

    TASK [install_communications : install_skype] **********************************
    ok: [0.0.0.0]

    TASK [install_communications : install_slack] **********************************
    ok: [0.0.0.0]

    TASK [install_editors : install_atom] ******************************************
    ok: [0.0.0.0]

    TASK [install_editors : install_sublime] ***************************************
    ok: [0.0.0.0]

    TASK [install_editors : install_textmate] **************************************
    ok: [0.0.0.0]

    TASK [install_editors : install_rmate] *****************************************
    ok: [0.0.0.0]

    TASK [install_editors : install_macvim] ****************************************
    ok: [0.0.0.0]

    TASK [install_electron : install_electron] *************************************
    ok: [0.0.0.0]

    TASK [install_erlang_elixir : Install erlang] **********************************
    ok: [0.0.0.0]

    TASK [install_iterm : install_iterm] *******************************************
    ok: [0.0.0.0]

    TASK [install_maria_db : install_alfred] ***************************************
    ok: [0.0.0.0]

    TASK [install_node : install_node] *********************************************
    ok: [0.0.0.0]

    TASK [install_node : install_nvm] **********************************************
    ok: [0.0.0.0]

    TASK [install_rbenv : install_rbenv] *******************************************
    ok: [0.0.0.0]

    TASK [install_redis : install_redis] *******************************************
    ok: [0.0.0.0]

    TASK [install_ruby_build : install_ruby-build] *********************************
    ok: [0.0.0.0]

    TASK [install_tmux : install_tmux] *********************************************
    ok: [0.0.0.0]

    TASK [install_tmux : Install tmux-switch-session] ******************************
    ok: [0.0.0.0]

    TASK [install_tmux : Install tmuxinator gem] ***********************************
    ok: [0.0.0.0]

    TASK [install_utilities : install_alfred] **************************************
    ok: [0.0.0.0]

    TASK [install_utilities : install_hyper] ***************************************
    ok: [0.0.0.0]

    TASK [install_utilities : Install virtualbox] **********************************
    ok: [0.0.0.0]

    TASK [install_utilities : Install vagrant] *************************************
    ok: [0.0.0.0]

    TASK [install_utilities : Install the vagrant-vbguest Vagrant plugin] **********
    changed: [0.0.0.0]

    TASK [install_utilities_command_line : Install wget] ***************************
    ok: [0.0.0.0]

    TASK [install_utilities_command_line : Install git] ****************************
    ok: [0.0.0.0]

    TASK [install_utilities_command_line : configure github] ***********************
    changed: [0.0.0.0]

    TASK [install_utilities_command_line : Install vtop] ***************************
    ok: [0.0.0.0]

    TASK [install_utilities_command_line : Install htop] ***************************
    ok: [0.0.0.0]

    TASK [install_utilities_command_line : Install reattach-to-user-namespace] *****
    ok: [0.0.0.0]

    TASK [install_utilities_command_line : Install mpd] ****************************
    ok: [0.0.0.0]

    TASK [install_utilities_command_line : Install lua] ****************************
    ok: [0.0.0.0]

    TASK [install_utilities_command_line : Install ffmpeg] *************************
    ok: [0.0.0.0]

    TASK [install_utilities_command_line : Install terminal-notifier] **************
    ok: [0.0.0.0]

    TASK [install_utilities_command_line : Install The Silver Searcher] ************
    ok: [0.0.0.0]

    TASK [install_utilities_command_line : Install bundler gem] ********************
    ok: [0.0.0.0]

    TASK [install_utilities_command_line : Install tree] ***************************
    ok: [0.0.0.0]

    TASK [install_utilities_command_line : Install lynx] ***************************
    ok: [0.0.0.0]

Not bad for less than 4 hours start to finish... Vastly better than installing / configuring all this crap by hand.
