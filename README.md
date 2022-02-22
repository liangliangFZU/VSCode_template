# VSCode_template

Contains some basic Visual Studio project templates.

## MSVC compiler options

Microsoft (R) C/C++ Optimizing Compiler Version 19.29.30140 for x64
Copyright (C) Microsoft Corporation. All rights reserved.

### C/C++ COMPILER OPTIONS

                              -OPTIMIZATION-

/O1 maximum optimizations (favor space) /O2 maximum optimizations (favor speed)
/Ob&lt;n&gt; inline expansion (default n=0) /Od disable optimizations (default)
/Og enable global optimization /Oi[-] enable intrinsic functions
/Os favor code space /Ot favor code speed
/Ox optimizations (favor speed)
/favor:&lt;blend|AMD64|INTEL64|ATOM&gt; select processor to optimize for, one of:
blend - a combination of optimizations for several different x64 processors
AMD64 - 64-bit AMD processors
INTEL64 - Intel(R)64 architecture processors
ATOM - Intel(R) Atom(TM) processors

                             -CODE GENERATION-

/Gu[-] ensure distinct functions have distinct addresses
/Gw[-] separate global variables for linker
/GF enable read-only string pooling /Gm[-] enable minimal rebuild
/Gy[-] separate functions for linker /GS[-] enable security checks
/GR[-] enable C++ RTTI /GX[-] enable C++ EH (same as /EHsc)
/guard:cf[-] enable CFG (control flow guard)
/guard:ehcont[-] enable EH continuation metadata (CET)
/EHs enable C++ EH (no SEH exceptions) /EHa enable C++ EH (w/ SEH exceptions)
/EHc extern "C" defaults to nothrow
(press &lt;return&gt; to continue)
/EHr always generate noexcept runtime termination checks
/fp:&lt;except[-]|fast|precise|strict&gt; choose floating-point model:
except[-] - consider floating-point exceptions when generating code
fast - "fast" floating-point model; results are less predictable
precise - "precise" floating-point model; results are predictable
strict - "strict" floating-point model (implies /fp:except)
/Qfast_transcendentals generate inline FP intrinsics even with /fp:except
/Qspectre[-] enable mitigations for CVE 2017-5753
/Qpar[-] enable parallel code generation
/Qpar-report:1 auto-parallelizer diagnostic; indicate parallelized loops
/Qpar-report:2 auto-parallelizer diagnostic; indicate loops not parallelized
/Qvec-report:1 auto-vectorizer diagnostic; indicate vectorized loops
/Qvec-report:2 auto-vectorizer diagnostic; indicate loops not vectorized
/GL[-] enable link-time code generation
/volatile:&lt;iso|ms&gt; choose volatile model:
iso - Acquire/release semantics not guaranteed on volatile accesses
ms - Acquire/release semantics guaranteed on volatile accesses
/GA optimize for Windows Application /Ge force stack checking for all funcs
/Gs[num] control stack checking calls /Gh enable \_penter function call
/GH enable \_pexit function call /GT generate fiber-safe TLS accesses
/RTC1 Enable fast checks (/RTCsu) /RTCc Convert to smaller type checks
/RTCs Stack Frame runtime checking /RTCu Uninitialized local usage checks
/clr[:option] compile for common language runtime, where option is:
pure : produce IL-only output file (no native executable code)
safe : produce IL-only verifiable output file
netcore : produce assemblies targeting .NET Core runtime
noAssembly : do not produce an assembly
nostdlib : ignore the system .NET framework directory when searching for assemblies
nostdimport : do not import any required assemblies implicitly
initialAppDomain : enable initial AppDomain behavior of Visual C++ 2002
(press &lt;return&gt; to continue)
implicitKeepAlive- : turn off implicit emission of System::GC::KeepAlive(this)
/fsanitize=address Enable address sanitizer codegen
/homeparams Force parameters passed in registers to be written to the stack
/GZ Enable stack checks (/RTCs) /Gv \_\_vectorcall calling convention
/arch:&lt;AVX|AVX2|AVX512&gt; minimum CPU architecture requirements, one of:
AVX - enable use of instructions available with AVX-enabled CPUs
AVX2 - enable use of instructions available with AVX2-enabled CPUs
AVX512 - enable use of instructions available with AVX-512-enabled CPUs
/QIntel-jcc-erratum enable mitigations for Intel JCC erratum
/Qspectre-load Enable spectre mitigations for all instructions which load memory
/Qspectre-load-cf Enable spectre mitigations for all control-flow instructions which load memory
/fpcvt:&lt;IA|BC&gt; FP to unsigned integer conversion compatibility
IA - results compatible with VCVTTSD2USI instruction
BC - results compatible with VS2017 and earlier compiler

                              -OUTPUT FILES-

/Fa[file] name assembly listing file /FA[scu] configure assembly listing
/Fd[file] name .PDB file /Fe&lt;file&gt; name executable file
/Fm[file] name map file /Fo&lt;file&gt; name object file
/Fp&lt;file&gt; name precompiled header file /Fr[file] name source browser file
/FR[file] name extended .SBR file /Fi[file] name preprocessed file
/Fd: &lt;file&gt; name .PDB file /Fe: &lt;file&gt; name executable file
/Fm: &lt;file&gt; name map file /Fo: &lt;file&gt; name object file
/Fp: &lt;file&gt; name .PCH file /FR: &lt;file&gt; name extended .SBR file
/Fi: &lt;file&gt; name preprocessed file
/Ft&lt;dir&gt; location of the header files generated for #import
/doc[file] process XML documentation comments and optionally name the .xdc file

                              -PREPROCESSOR-

/AI&lt;dir&gt; add to assembly search path /FU&lt;file&gt; forced using assembly/module
/C don't strip comments /D&lt;name&gt;{=|#}&lt;text&gt; define macro
/E preprocess to stdout /EP preprocess to stdout, no #line
/P preprocess to file /Fx merge injected code to file
/FI&lt;file&gt; name forced include file /U&lt;name&gt; remove predefined macro
/u remove all predefined macros /I&lt;dir&gt; add to include search path
/X ignore "standard places"
/PH generate #pragma file_hash when preprocessing
/PD print all macro definitions

                                -LANGUAGE-

/std:&lt;c++14|c++17|c++latest&gt; C++ standard version
c++14 - ISO/IEC 14882:2014 (default)
c++17 - ISO/IEC 14882:2017
c++latest - latest draft standard (feature set subject to change)
/permissive[-] enable some nonconforming code to compile (feature set subject to change) (on by default)
/Ze enable extensions (default) /Za disable extensions
/ZW enable WinRT language extensions /Zs syntax check only
/Zc:arg1[,arg2] C++ language conformance, where arguments can be:
forScope[-] enforce Standard C++ for scoping rules
wchar_t[-] wchar_t is the native type, not a typedef
auto[-] enforce the new Standard C++ meaning for auto
trigraphs[-] enable trigraphs (off by default)
rvalueCast[-] enforce Standard C++ explicit type conversion rules
strictStrings[-] disable string-literal to [char|wchar_t]\*
conversion (off by default)
implicitNoexcept[-] enable implicit noexcept on required functions
threadSafeInit[-] enable thread-safe local static initialization
inline[-] remove unreferenced function or data if it is
COMDAT or has internal linkage only (off by default)
sizedDealloc[-] enable C++14 global sized deallocation
functions (on by default)
throwingNew[-] assume operator new throws on failure (off by default)
referenceBinding[-] a temporary will not bind to an non-const
lvalue reference (off by default)
(press &lt;return&gt; to continue)
twoPhase- disable two-phase name lookup
ternary[-] enforce C++11 rules for conditional operator (off by default)
noexceptTypes[-] enforce C++17 noexcept rules (on by default in C++17 or later)
alignedNew[-] enable C++17 alignment of dynamically allocated objects (on by default)
hiddenFriend[-] enforce Standard C++ hidden friend rules (implied by /permissive-)
externC[-] enforce Standard C++ rules for 'extern "C"' functions (implied by /permissive-)
lambda[-] better lambda support by using the newer lambda processor (off by default)
tlsGuards[-] generate runtime checks for TLS variable initialization (on by default)
zeroSizeArrayNew[-] call member new/delete for 0-size arrays of objects (on by default)
/await enable resumable functions extension
/await:strict enable standard C++20 coroutine support with earlier language versions
/constexpr:depth&lt;N&gt; recursion depth limit for constexpr evaluation (default: 512)
/constexpr:backtrace&lt;N&gt; show N constexpr evaluations in diagnostics (default: 10)
/constexpr:steps&lt;N&gt; terminate constexpr evaluation after N steps (default: 100000)
/Zi enable debugging information /Z7 enable old-style debug info
/Zo[-] generate richer debugging information for optimized code (on by default)
/ZH:[MD5|SHA1|SHA_256] hash algorithm for calculation of file checksum in debug info (default: MD5)
/Zp[n] pack structs on n-byte boundary /Zl omit default library name in .OBJ
/vd{0|1|2} disable/enable vtordisp /vm&lt;x&gt; type of pointers to members
/std:&lt;c11|c17&gt; C standard version
c11 - ISO/IEC 9899:2011
c17 - ISO/IEC 9899:2018
/ZI enable Edit and Continue debug info
/openmp enable OpenMP 2.0 language extensions
/openmp:experimental enable OpenMP 2.0 language extensions plus select OpenMP 3.0+ language extensions
/openmp:llvm OpenMP language extensions using LLVM runtime

                              -MISCELLANEOUS-

@&lt;file&gt; options response file /?, /help print this help message
/bigobj generate extended object format /c compile only, no link
/errorReport:option deprecated. Report internal compiler errors to Microsoft
none - do not send report
(press &lt;return&gt; to continue)
prompt - prompt to immediately send report
queue - at next admin logon, prompt to send report (default)
send - send report automatically
/FC use full pathnames in diagnostics /H&lt;num&gt; max external name length
/J default char type is unsigned
/MP[n] use up to 'n' processes for compilation
/nologo suppress copyright message /showIncludes show include file names
/Tc&lt;source file&gt; compile file as .c /Tp&lt;source file&gt; compile file as .cpp
/TC compile all files as .c /TP compile all files as .cpp
/V&lt;string&gt; set version string /Yc[file] create .PCH file
/Yd put debug info in every .OBJ /Yl[sym] inject .PCH ref for debug lib
/Yu[file] use .PCH file /Y- disable all PCH options
/Zm&lt;n&gt; max memory alloc (% of default) /FS force to use MSPDBSRV.EXE
/source-charset:&lt;iana-name&gt;|.nnnn set source character set
/execution-charset:&lt;iana-name&gt;|.nnnn set execution character set
/utf-8 set source and execution character set to UTF-8
/validate-charset[-] validate UTF-8 files for only legal characters
/fastfail[-] enable fast-fail mode /JMC[-] enable native just my code
/presetPadding[-] zero initialize padding for stack based class types
/volatileMetadata[-] generate metadata on volatile memory accesses

                                -LINKING-

/LD Create .DLL /LDd Create .DLL debug library
/LN Create a .netmodule /F&lt;num&gt; set stack size
/link [linker options and libraries] /MD link with MSVCRT.LIB
/MT link with LIBCMT.LIB /MDd link with MSVCRTD.LIB debug lib
/MTd link with LIBCMTD.LIB debug lib

                              -CODE ANALYSIS-

(press &lt;return&gt; to continue)
/analyze[-] Enable native analysis /analyze:quiet[-] No warning to console
/analyze:log&lt;name&gt; Warnings to file /analyze:autolog Log to _.pftlog
/analyze:autolog:ext&lt;ext&gt; Log to _.&lt;ext&gt;/analyze:autolog- No log file
/analyze:WX- Warnings not fatal /analyze:stacksize&lt;num&gt; Max stack frame
/analyze:max_paths&lt;num&gt; Max paths /analyze:only Analyze, no code gen

                              -DIAGNOSTICS-

/diagnostics:&lt;args,...&gt; controls the format of diagnostic messages:
classic - retains prior format
column[-] - prints column information
caret[-] - prints column and the indicated line of source
/Wall enable all warnings /w disable all warnings
/W&lt;n&gt; set warning level (default n=1)
/Wv:xx[.yy[.zzzzz]] disable warnings introduced after version xx.yy.zzzzz
/WX treat warnings as errors /WL enable one line diagnostics
/wd&lt;n&gt; disable warning n /we&lt;n&gt; treat warning n as an error
/wo&lt;n&gt; issue warning n once /w&lt;l&gt;&lt;n&gt; set warning level 1-4 for n
/external:I &lt;path&gt; - location of external headers
/external:env:&lt;var&gt; - environment variable with locations of external headers
/external:anglebrackets - treat all headers included via &lt;&gt; as external
/external:W&lt;n&gt; - warning level for external headers
/external:templates[-] - evaluate warning level across template instantiation chain
/sdl enable additional security features and warnings
