node('centos7Agent'){
    wrap([$class: 'MaskPasswordsBuildWrapper', varPasswordPairs: [[password: 'tsweet', var: 'myPassword']]]) {
    def test='myPassword'
    echo test
    sh '''if [$test -eq $tsweet ]; then 
            echo I match! 
        else echo No match 
        fi'''
    }
}