module Main where

--- Fibonachi: 1 -> 0; 2 -> 1; 3 -> 1; 4 -> 2; 5 -> 3 ... 
--- if < 0 then -1 "error"
fib :: Int -> Int
fib a =
  if a < 0
    then - 1
    else if a == 1
           then 0
           else
             let
               stop p = p < 4 

               go bef1 bef2 p = if stop p
                                  then (bef1 + bef2)
                                  else let bef1' = bef2
                                           bef2' = bef1 + bef2
                                           p' = p - 1
                                       in go bef1' bef2' p'
             in go 0 1 a

main = print (fib 5)
