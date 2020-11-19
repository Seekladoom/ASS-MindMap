 The PyonFX Library Documentation

# Quick Start Guide

## First of all

### ASS format

### Python3 scripting language

## Windows

## Ubuntu/Debian

## Fedora

## Arch Linux

## openSUSE

## macOS

## Installation - Extra Step

## Starting

## Tips

# The PyonFX Library Reference

## Ass Core

### class pyonfx.ass_core.Meta

#### wrap_style

#### scaled_border_and_shadow

#### play_res_x

#### play_res_y

#### audio

#### video

### class pyonfx.ass_core.Style

#### fontname

#### fontsize

#### color1

#### alpha1

#### color2

#### alpha2

#### color3

#### alpha3

#### color4

#### alpha4

#### bold

#### italic

#### underline

#### strikeout

#### scale_x

#### scale_y

#### spacing

#### angle

#### border_style

#### outline

#### shadow

#### alignment

#### margin_l

#### margin_r

#### margin_v

#### encoding

### class pyonfx.ass_core.Char

#### i

#### word_i

#### syl_i

#### syl_char_i

#### start_time

#### end_time

#### duration

#### styleref

#### text

#### inline_fx

#### prespace

#### postspace

#### width

#### height

#### x

#### y

#### left

#### center

#### right

#### top

#### middle

#### bottom

### class pyonfx.ass_core.Syllable

#### i

#### word_i

#### start_time

#### end_time

#### duration

#### styleref

#### text

#### tags

#### inline_fx

#### prespace

#### postspace

#### width

#### height

#### x

#### y

#### left

#### center

#### right

#### top

#### middle

#### bottom

### class pyonfx.ass_core.Word

#### i

#### start_time

#### end_time

#### duration

#### styleref

#### text

#### prespace

#### postspace

#### width

#### height

#### x

#### y

#### left

#### center

#### right

#### top

#### middle

#### bottom

### class pyonfx.ass_core.Line

#### i

#### comment

#### layer

#### start_time

#### end_time

#### duration

#### leadin

#### leadout

#### style

#### styleref

#### actor

#### margin_l

#### margin_r

#### margin_v

#### effect

#### raw_text

#### text

#### width

#### height

#### ascent

#### descent

#### internal_leading

#### external_leading

#### x

#### y

#### left

#### center

#### right

#### top

#### middle

#### bottom

#### words

#### syls

#### chars

#### copy()

### class pyonfx.ass_core.Ass(path_input='', path_output='Output.ass', keep_original=True, extended=True, vertical_kanji=True)

#### path_input

#### path_output

#### meta

#### styles

#### lines

#### get_data()

#### write_line(line)

#### save(quiet=False)

#### open_aegisub()

#### open_mpv(video_path='', video_start='', full_screen=False)

## Convert Functions

### class pyonfx.convert.Convert

#### static time(ass_ms)

#### static coloralpha(ass_r_a, g='', b='', a='')

#### static text_to_shape(obj, fscx=None, fscy=None)

#### static text_to_clip(obj, an=5, fscx=None, fscy=None)

#### static text_to_pixels(obj, supersampling=8)

#### static shape_to_pixels(shape, supersampling=8)

## Shape Functions

### class pyonfx.shape.Shape(drawing_cmds)

#### has_error()

#### map(fun)

#### bounding()

#### move(x=None, y=None)

#### flatten(tolerance=1.0)

#### split(max_len=16, tolerance=1.0)

#### static ring(out_r, in_r)

#### static ellipse(w, h)

#### static heart(size, offset=0)

#### static star(edges, inner_size, outer_size)

#### static glance(edges, inner_size, outer_size)

#### static rectangle(w=1, h=1)

#### static triangle(size)

## Utils

### class pyonfx.utils.Utils

### static interpolate(pct, val1, val2, acc=1.0)

### class pyonfx.utils.FrameUtility(start_time, end_time, fr=41.71)

### classpyonfx.utils.ColorUtility(lines, offset=0)

### get_color_change(line, c1=None, c3=None, c4=None)

### get_fr_color_change(line, c1=None, c3=None, c4=None)
