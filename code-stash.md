# Code stash
A pice of code that:
- might be useful in the future
- Interesting, but no time to read now

## Chunk while
Group adjacent thing together according to the functions
Same thing in ramdajs: [groupWith](https://ramdajs.com/docs/#groupWith)

```gleam
fn chunk_while(list: List(a), while fun: fn(a, a) -> Bool) -> List(List(a)) {
    case list {
        [] -> []
        [first, ..rest] -> do_chunk_while(rest, fun, first, [], [])
    }
}

fn do_chunk_while(list, fun, last, curr, acc) {
    case list {
        [] -> list.reverse([list.reverse([last, ..curr]), ..acc])
        [next, ..rest] -> {
            let curr = [last, ..curr]
            case fun(last, next) {
                True -> do_chunk_while(rest, fun, next, curr, acc)
                False -> do_chunk_while(rest, fun, next, [], [list.reverse(curr), ..acc], )
            }
        }
    }
}
```
