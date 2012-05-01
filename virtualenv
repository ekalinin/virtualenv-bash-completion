# virtualenv --help

have virtualenv && {
_virtualenv() {
    local cur prev opts
    COMPREPLY=()
    cur="${COMP_WORDS[COMP_CWORD]}"
    prev="${COMP_WORDS[COMP_CWORD-1]}"
    opts=$(virtualenv --help | grep -P -o "(\s(-\w{1}|--[\w-]*=?)){1,2}" | \
                sort | uniq | grep -v "extra\-search\-dir$")

    if [[ ${cur} == -* ]] ; then
        COMPREPLY=( $(compgen -W "${opts}" -- ${cur}) )
        return 0
    fi
}
complete -F _virtualenv virtualenv
}

# Local variables:
# mode: shell-script
# sh-basic-offset: 4
# sh-indent-comment: t
# indent-tabs-mode: nil
# End:
# ex: ts=4 sw=4 et filetype=sh
