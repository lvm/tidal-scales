TidalCycles / Haskell modules with Scales and Chords.

# Requirements

ghc >= 7.10  
tidal >= 0.8  

### installation

```shell
git clone https://github.com/lvm/tidal-scales
cd tidal-scales
cabal clean && cabal configure && cabal build && cabal install
```

### Usage

To see the contents, you can use `ghci`'s `:browse`

```haskell
Prelude> :browse Sound.Tidal.Scales
Sound.Tidal.Scales._Maj :: [Int]
Sound.Tidal.Scales._min :: [Int]
Sound.Tidal.Scales.aeolian :: [Int]
Sound.Tidal.Scales.ahirbhairav :: [Int]
Sound.Tidal.Scales.aug :: [Int]
Sound.Tidal.Scales.augmented :: [Int]
Sound.Tidal.Scales.augmented2 :: [Int]
Sound.Tidal.Scales.bartok :: [Int]
Sound.Tidal.Scales.bhairav :: [Int]
Sound.Tidal.Scales.chinese :: [Int]
Sound.Tidal.Scales.chromatic :: [Int]
Sound.Tidal.Scales.dim :: [Int]
Sound.Tidal.Scales.dim7 :: [Int]
Sound.Tidal.Scales.diminished :: [Int]
Sound.Tidal.Scales.diminished2 :: [Int]
Sound.Tidal.Scales.dom7 :: [Int]
Sound.Tidal.Scales.dorian :: [Int]
Sound.Tidal.Scales.egyptian :: [Int]
Sound.Tidal.Scales.eleven :: [Int]
Sound.Tidal.Scales.enigmatic :: [Int]
Sound.Tidal.Scales.evelenSharp :: [Int]
Sound.Tidal.Scales.five :: [Int]
Sound.Tidal.Scales.gong :: [Int]
Sound.Tidal.Scales.harmonicMajor :: [Int]
Sound.Tidal.Scales.harmonicMinor :: [Int]
Sound.Tidal.Scales.hexAeolian :: [Int]
Sound.Tidal.Scales.hexDorian :: [Int]
Sound.Tidal.Scales.hexMajor6 :: [Int]
Sound.Tidal.Scales.hexMajor7 :: [Int]
Sound.Tidal.Scales.hexPhrygian :: [Int]
Sound.Tidal.Scales.hexSus :: [Int]
Sound.Tidal.Scales.hindu :: [Int]
Sound.Tidal.Scales.hirajoshi :: [Int]
Sound.Tidal.Scales.hungarianMinor :: [Int]
Sound.Tidal.Scales.indian :: [Int]
Sound.Tidal.Scales.ionian :: [Int]
Sound.Tidal.Scales.iwato :: [Int]
Sound.Tidal.Scales.jiao :: [Int]
Sound.Tidal.Scales.kumai :: [Int]
Sound.Tidal.Scales.leadingWhole :: [Int]
Sound.Tidal.Scales.locrian :: [Int]
Sound.Tidal.Scales.locrianMajor :: [Int]
Sound.Tidal.Scales.lydian :: [Int]
Sound.Tidal.Scales.lydianMinor :: [Int]
Sound.Tidal.Scales.m11 :: [Int]
Sound.Tidal.Scales.m11sharp :: [Int]
Sound.Tidal.Scales.m13 :: [Int]
Sound.Tidal.Scales.m6 :: [Int]
Sound.Tidal.Scales.m6by9 :: [Int]
Sound.Tidal.Scales.m7flat5 :: [Int]
Sound.Tidal.Scales.m7flat9 :: [Int]
Sound.Tidal.Scales.m7sharp5 :: [Int]
Sound.Tidal.Scales.m7sharp5flat9 :: [Int]
Sound.Tidal.Scales.m7sharp9 :: [Int]
Sound.Tidal.Scales.m9 :: [Int]
Sound.Tidal.Scales.m9sharp5 :: [Int]
Sound.Tidal.Scales.maj11 :: [Int]
Sound.Tidal.Scales.maj9 :: [Int]
Sound.Tidal.Scales.majPent :: [Int]
Sound.Tidal.Scales.major :: [Int]
Sound.Tidal.Scales.major7 :: [Int]
Sound.Tidal.Scales.marva :: [Int]
Sound.Tidal.Scales.melodicMajor :: [Int]
Sound.Tidal.Scales.melodicMinor :: [Int]
Sound.Tidal.Scales.melodicMinorDesc :: [Int]
Sound.Tidal.Scales.minPent :: [Int]
Sound.Tidal.Scales.minor :: [Int]
Sound.Tidal.Scales.minor7 :: [Int]
Sound.Tidal.Scales.mixolydian :: [Int]
Sound.Tidal.Scales.msharp5 :: [Int]
Sound.Tidal.Scales.neapolitanMajor :: [Int]
Sound.Tidal.Scales.neapolitanMinor :: [Int]
Sound.Tidal.Scales.nine :: [Int]
Sound.Tidal.Scales.nineSharp5 :: [Int]
Sound.Tidal.Scales.nineSus4 :: [Int]
Sound.Tidal.Scales.one :: [Int]
Sound.Tidal.Scales.pelog :: [Int]
Sound.Tidal.Scales.phrygian :: [Int]
Sound.Tidal.Scales.plus :: [Int]
Sound.Tidal.Scales.prometheus :: [Int]
Sound.Tidal.Scales.purvi :: [Int]
Sound.Tidal.Scales.ritusen :: [Int]
Sound.Tidal.Scales.romanianMinor :: [Int]
Sound.Tidal.Scales.scriabin :: [Int]
Sound.Tidal.Scales.sevenFlat10 :: [Int]
Sound.Tidal.Scales.sevenFlat5 :: [Int]
Sound.Tidal.Scales.sevenFlat9 :: [Int]
Sound.Tidal.Scales.sevenSharp5 :: [Int]
Sound.Tidal.Scales.sevenSharp5flat9 :: [Int]
Sound.Tidal.Scales.sevenSus2 :: [Int]
Sound.Tidal.Scales.sevenSus4 :: [Int]
Sound.Tidal.Scales.shang :: [Int]
Sound.Tidal.Scales.sharp5 :: [Int]
Sound.Tidal.Scales.six :: [Int]
Sound.Tidal.Scales.sixby9 :: [Int]
Sound.Tidal.Scales.spanish :: [Int]
Sound.Tidal.Scales.superLocrian :: [Int]
Sound.Tidal.Scales.sus2 :: [Int]
Sound.Tidal.Scales.sus4 :: [Int]
Sound.Tidal.Scales.thirteen :: [Int]
Sound.Tidal.Scales.todi :: [Int]
Sound.Tidal.Scales.whole :: [Int]
Sound.Tidal.Scales.yu :: [Int]
Sound.Tidal.Scales.zhi :: [Int]
```

In the TidalCycles Environment you can use it like this:

```haskell
import Sound.Tidal.Scales

midi7 $ n "c c c"
# n ((+) <$> "c c c" <*> (listToPat _min))
```
