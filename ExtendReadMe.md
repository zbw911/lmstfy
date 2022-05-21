``` go
var signals = [...]string{
    // 这里省略N行。。。。

    /** 兼容windows start */
    16: "SIGUSR1",
    17: "SIGUSR2",
    18: "SIGTSTP",
    /** 兼容windows end */
}

/** 兼容windows start */
func Kill(...interface{}) error {
    return nil;
}
const (
    SIGUSR1 = Signal(16)
    SIGUSR2 = Signal(17)
    SIGTSTP = Signal(18)
)
/** 兼容windows end */

// https://learnku.com/articles/51696

```


grafana: https://grafana.com/grafana/dashboards/12748

-c config/demo-conf.toml